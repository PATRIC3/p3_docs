
.. _cli::p3-extract-gto:

##############
p3-extract-gto
##############

.. highlight:: perl


.. _cli::Create-a-gto-file-of-a-Patric-genome:

************************************
Create a gto file of a Patric genome
************************************



.. code-block:: perl

     p3-extract-gto genome-id [options]
 
     Create a gto file from a patric genome.
 =cut


use strict;
use P3DataAPI;
use Data::Dumper;
use gjoseqlib;
use GenomeTypeObject;

use Getopt::Long::Descriptive;

my($opt, $usage) = describe_options("%c %o genome-id [ > genome.gto ]",
                                    ["output|o=s", "Write to this output file instead of stdout"],
                                    ["help|h", "Show this help message"]);

print($usage->text), exit  if $opt->help;
die($usage->text) if (@ARGV != 1);

my @ids;
my $type;

my $gid = shift;

my $d = P3DataAPI->new();

my $gto = GenomeTypeObject->new();

my @res = $d->query("genome", ["eq", "genome_id", $gid],
                    ["select", "genome_id", "genome_name", "taxon_id", "taxon_lineage_names"],
                   );

@res == 1 or die "Cannot find genome $gid\n";

my $gname = $res[0]->{genome_name};
my $tax_id = $res[0]->{taxon_id};
my $tax = $res[0]->{taxon_lineage_names};
shift @$tax if $tax->[0] eq 'root' || $tax->[0] eq 'cellular organisms';
my $dom = $tax->[0];
my $domain = $dom =~ /^Arch/i      ? 'Archaea'
    : $dom =~ /^Bact/i      ? 'Bacteria'
    : $dom =~ /^Eu[ck]a/i   ? 'Eukaryota'
    : $dom =~ /^Vir/i       ? 'Virus'
    : $dom =~ /^Environ/i   ? 'Environmental Sample'
    : $dom =~ /^Un\S\* Env/i ? 'Environmental Sample'
    :                         'Unknown';
my $taxonomy = join("; ", @$tax, $gname);

@res = $d->query("taxonomy", ["eq", "taxon_id", $tax_id], ["select", "genetic_code"]);
@res == 1 or die "Cannot find taxon_id $tax_id\n";

my $genetic_code = $res[0]->{genetic_code};

$gto->set_metadata({
    id => $gid,
    scientific_name => $gname,
    genetic_code => $genetic_code,
    ncbi_taxonomy_id => $tax_id,
    taxonomy => $taxonomy,
    domain => $domain,
});

my(@fields) = qw(feature_type
                 patric_id
                 segments
                 aa_sequence
                 accession
                 location
                 strand
                 product
                 uniprotkb_accession
                 gi
                 gene
                 refseq_locus_tag
                 );

@res = $d->query("genome_feature",
                 ["select", @fields],
                 ["ne", "feature_type", "source"],
                 ["eq", "annotation", "PATRIC"],
                 ["eq", "genome_id", $gid],
                );

for my $ent (@res)
{
    next if $ent->{patric_id} eq '';


.. code-block:: perl

     my @loc;
     for my $lent (@{$ent->{segments}})
     {
         if (my($l, $r) = ($lent =~ /^(\d+)\.\.(\d+)/))
         {
             my $len = $r - $l + 1;
             my $start = $l;
             if ($ent->{strand} eq '-')
             {
                 $start = $r;
             }
             push(@loc, [$ent->{accession}, $start, $ent->{strand}, $len]);
         }
         else
         {
             die "Could not parse location '$lent'\n";
         }
     }
     my $type = $ent->{feature_type};
 
     $type = 'rna' if ($type eq 'tRNA' || $type eq 'rRNA');
     my $aliases = [];
     my $alias_pairs = [];
     if (my $v = $ent->{gi})
     {
         push(@$aliases, "gi|$v");
         push(@$alias_pairs, [gi => $v]);
     }
     if (my $v = $ent->{gene})
     {
         push(@$aliases, $v);
         push(@$alias_pairs, [gene => $v]);
     }
     if (my $v = $ent->{refseq_locus_tag})
     {
         push(@$aliases, $v);
         push(@$alias_pairs, [locus_tag => $v]);
     }
 
 
     my $feat = {
         id => $ent->{patric_id},
         location => [@loc],
         type => $type,
         function => $ent->{product},
         ($ent->{aa_sequence} eq '' ? () : (protein_translation => $ent->{aa_sequence} )),
         aliases => $aliases,
         alias_pairs => $alias_pairs,
         annotations => [],
         family_assignments => [],
         similarity_associations => [],
         proposed_functions => [],
     };
     push(@{$gto->{features}}, $feat);


}

@res = $d->query("genome_sequence",
                 ["select", "genome_id", "accession", "sequence"],
                 ["eq", "genome_id", $gid],
                );

for my $ent (@res)
{
    push(@{$gto->contigs},
     {
         dna => $ent->{sequence},
         genetic_code => $genetic_code,
         id => $ent->{accession},
     });
}

$gto->destroy_to_file($opt->output);

