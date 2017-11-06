Reconstructing Genomes from Metagenomic Samples Using the RAST Binning Service (RBS)
====================================================================================

The ability to reconstruct fairly complete genomes from metagenomic
samples is almost certainly a key technology that will accelerate our
characterization of the tree of life. A number of research groups have
now generated valuable reconstructions of genomes from metagenomic
samples, and this is having an impact on estimating genomic sequences
for unculturable organims. For background we particularly recommend

         Recovery of nearly 8,000 metagenome-assembled genomes 
         substantially expands the tree of life.

by

         Parks DH, Rinke C, Chuvochina M, Chaumeil PA, Woodcroft BJ, Evans PN, 
         Hugenholtz P, Tyson GW. Nat Microbiol. 2017 
         PMID: 28894102

but there have been several other excellent efforts that have been
reported over the last few years.

RBS is a server that grew out of the RAST annotation project; it is now
supported and maintained as part of the PATRIC project.

The Server: an Overview
-----------------------

As input to the server, a user supplies a metagenomic sample in one of
the following forms:

#. two files containing paired-end reads,
#. the ID for a sample in the sample archives, or
#. a file of contigs produced by a cross-assembler. More precisely it
   can be a set of *cross-assemblies*, where each cross-assembly was
   constructed from the reads associated with one or more samples. It
   should be noted that each cross-assembly should include an estimate
   of coverage for every contig. You can use
   `crAss <https://edwards.sdsu.edu/crass/>`__ to generate the input
   cross-assemblies, you can use your favorite assembler software, or
   you can use the assembly server in the PATRIC web site.


The output is a set of *Genome Packages*. Each genome package is a
*Rast Genome* along with an *Evaluation Report* which estimates the
quality of the RAST genome.

The goal is to reconstruct complete (or near-complete) genomes from the
sample data. We will constrain ourselves to only extracting genomes with
an average coverage of at least 20, but you may wish to change that
somewhat arbitrary value. In any event, you should note that, at 20-fold
coverage, the regions in the actual genome that contain no large repeats
tend to be unbroken. Reconstructing a complete genome including the
large repeats is usually quite difficult, so we shoot for capturing the
regions between large repeats.

It should be noted that the number of genomes that we expect to extract
will depend on the samples we use as input. If we wish to explore the
proposed technology, it would make sense to begin with a very limited
collection of samples. On the other hand, if the goal were to extract as
many new gnomes as possible, one might select hundreds (or even
thousands) of samples as input. You should carefully note that this
document describes one approach to extracting genomes from samples.
There are a number of approaches emerging, and it is likely that aspects
of the process we describe may well turn out to be non-optimal. We do
hope that you will explore the approach and have fun in the process.

Here then is basically how we build the reconstructed genomes.

Step 1: Construct a Representative Collection of a Universal Protein
--------------------------------------------------------------------

First, pick a functional role that satisfies the following criteria:

#. Exactly one gene encodes the role in all (or at least most)
   prokaryotic genomes.
#. A role encoded by a long gene is preferred.


We picked

::

      Phenylalanyl-tRNA synthetase alpha chain (EC 6.1.1.20)

but there are other good choices.
Once we have selected a role, which we will call the *seed role*, we
construct a blast database containing a representative collection of
protein sequences that implement the seed role. This can be done using
`command-line access to the PATRIC collection of genomic
data <PATRIC-tutorials>`__.
We recommend using the SEEDtk routine

::

       bins_protein_database -R IdOfProtein OutputFileName

to compute a representative subset of your collection (which should be
fairly large). This script uses the PATRIC database to find all
occurrences of the identified protein. For Phenylalanyl-tRNA synthetase
alpha chain, the command would be

::

       bins_protein_database -R PhenTrnaSyntAlph seed_protein.fna

You can, of course, use any genome database to find the proteins and any
utility that produces a DNA fasta file of the relevant sequences. In our
program, the sequence ID in the FASTA file is the feature ID, and the
comment is the genome ID and scientific name.

Step 2: For Each Sample, Construct a set of Contig Bins
-------------------------------------------------------

The second step is to find all instances of the seed role in your
collection of cross-assemblies. This is done using blast. For each
sample you blast the representative set of instances of the seed role
against the cross-assembly associated with the sample. Filter out hits
which do not adequately cover the known seed role instance. Similarly,
remove hits against contigs that have less that 20-fold average
coverage. The hits that remain each represent a **bin** that will
eventually be expanded into a reconstructed genome. A bin is normally
thought of as containing a single genome, but when we cannot reasonably
resolve two bins, we occasionally merge them into one This data is
represented by a table containing

-  Bin Id
-  Sample Id
-  Contig Id
-  Start of hit
-  End of hit
-  Coverage of contig containing hit


Step 3: For Each Sample, Compute a Set of Reference Genomes
-----------------------------------------------------------

We have computed a set of bins, where each bin conceptually contains a
single *seed role* and the contig that contains that seed role. Our
overall objective is to determine which contigs from the cross-assembly
associated with the sample should be placed into each bin. That is, we
need to split the contig pool into subsets that go with each bin, and an
extra set of contigs that could not be placed (there may be many of
these coming from the non-abundant organisms included in the sample, as
well as those contigs whose placement would be ambiguous). There are
several possible strategies that could be used to place contigs into
bins. We have elected to use *reference genomes*. This involves
associating a known, sequenced reference genome with each of the bins.
These reference genomes play a central role in the next step, which
involves actually splitting up the pool of contigs in the
cross-assembly.

So, how should we go about assigning a sequenced reference genome to
each bin? We will attempt to find a reference genome that is
phylogenetically close to each bin. To be useful, the reference genome
will need to be substantially closer to the genome represented by the
bin than to any of the genomes represented by other bins. Here we can
used estimates of phylogenetic distance based on the instances of the
seed roles that are stored in the bins. It is clear that in many
situations, it will be impossible to find such a discriminating genome
from existing genome repositories. When a discriminating reference
genome cannot be found, the corresponding bin should be marked and
placed aside (until a larger collection of potential reference genomes
containing a useful reference can be generated).

We pick the most dsicriminating reference genome for each bin, but
nothing prohibits one from selecting multiple reference genomes for a
bin.

Step 4: For Each Sample, Place Contigs Into Bins
------------------------------------------------

Once reference genomes have been determined for each bin, we can
partition the contigs from the cross-assembly for each sample into the
bins. The use of reference bins involves computing some measure of the
similarity between a contig and the set of contigs in reference
genomes. This similarity measure can be based on any of a number of
algorithms, including the use of blast scores or the number of k-mers
in common. Assuming that we have a suitable measure, we can build a
scheme for partitioning the contgs in a cross-assembly.
For our purposes, we measure the similarity between two DNA contigs as
follows:

#. We translate the DNA to protein sequence (using 6-frames).
#. We count the number of amino acid 12-mers in common, and this is the
   score.
#. We consider the two DNA contigs as similar if they generate a score
   of 10 or more amino acid 12-mers.

We consider the similarity score beween one contig and a set of contigs
to be the maximum score between the contig and a contig from the set.

A contig **C** should be copied into bin **B** if and only if

#. the similarity of **C** against the contigs of the reference genomes
   for **B** exceeds a specified threshold, and it is greater than the
   similarity to other reference genomes. That is, **C** is put into the
   bin belonging to reference genome **G** if **C** is most similar to
   **G** and the similarity exceeds the threshold.
#. the difference in coverage between **C** and the average coverage in
   the similar contig from **B** is small.

Using this simple logic, we have experimented with a range of
thresholds.

Step 5: Evaluate the Quality of Each Bin
----------------------------------------

At this point, each bin contains a set of contigs that have tentatively
been labeled as coming from a single clonal population. There are
numerous possible sources of error, so how might we evaluate the quality
of a bin? Fortunately, several such tools exist. The most notable is
`checkM <http://genome.cshlp.org/content/early/2015/05/14/gr.186072.114>`__
(which we have found extremely useful):

        Parks DH, Imelfort M, Skennerton CT, Hugenholtz P, Tyson GW.
        2014.  Assessing the quality of microbial genomes recovered from
        isolates, single cells, and metagenomes.  Genome Research, 25:
        1043-1055.

We have written a tool that can be used to produce a single score that
measures the quality of a prokaryotic genome. Using these tools, one can
simply keep only high-scoring bins. This is an important point: as long
as your quality assessments are reasonably accurate, you can throw out
numerous bins and still be able to harvest thousands of new, fairly
accurate, genomes.

Step 6: For Each Bin, Remove Questionable Contigs
-------------------------------------------------

At the end of Step 5, we have accumulated a set of bins, along with
estimates of quality. We have developed a simple test for attempting to
spot contaminating contigs, so we run our algorithm, removing highly
questionable contigs (when such removals improve our estimates of
quality).

Step 7: Annotate High-Quality Bins
----------------------------------

We submit the contigs in each high-quality bin to the PATRIC server to
annotate the genome associated with the bin.

Step 8: For Each High-Quality Bin, Construct a Metabolic Model
--------------------------------------------------------------

For each annotated, high-quality bin, we compute an estimate of the
reaction network. We use this network as a means for evaluating the
quality of the annotations, as well as the overall accuracy of the bin.

Step 9: Estimate Taxonomy
-------------------------

For each high-quality bin, we estimate taxonomy using several of the
widely-available taxonomy servers (and one of our own).

Step 10: For Each High-Quality Bin, Generate a Skeletal Paper
-------------------------------------------------------------

We plan to generate genome papers for at least a subset of the
high-quality bins. To do this, we will use `the Genome Papers web
site <http://www.genomepapers.org>`__.

Summary
-------

In this document, we sketch out a plan for reconstructing thousands of
genomes from metagenomic samples. There are several alternative plans
being developed by the research community. Here is a brief summary of a
plan implemented by a European team that included Bjorn Nielsen, Dusko
Ehrlich and Peer Bork (see `"Identification and Assembly of Genomes and
Genetic Elements in Complex Metagenomic Samples Without Using Reference
Genomes" <https://www.researchgate.net/publication/264156295_Identification_and_assembly_of_genomes_and_genetic_elements_in_complex_metagenomic_samples_without_using_reference_genomes>`__).

          DNA from a series of independent biological samples from
          microbial communities, here originating from the human gut
          microbiome, is extracted and shotgun sequenced. Genes assembled
          and identified in individual samples are then integrated to form
          a cross-sample, nonredundant gene catalog. The abundance profile
          of each gene in the catalog is assessed by counting the matching
          sequence reads in each sample. To facilitate co-abundance
          clustering of large gene catalogs, we used random seed genes as
          'baits' for identifying groups of genes that correlate (PCC >
          0.9) to the abundance profile of the bait genes. The fixed PCC
          distance threshold is called a canopy. To
          center the canopy on a co-abundance gene group (CAG), the median
          gene abundance profile of the genes within the original seed
          canopy (or subsequent canopies) is used
          iteratively to recapture a new canopy until it settles on a
          particular profile. The gene content of a
          settled canopy is named a metagenomic
          species (MGS) if it contains 700 or more genes. The smaller
          groups remain referred to as CAGs. Sequence reads from
          individual samples that map to the MGS genes and their contigs
          are then extracted and used to assembly a draft genome sequence
          for an MGS; we refer to this process as MGS-augmented genome
          assembly. The use of sample-specific sequence reads in the
          assemblies helps discriminate between closely related strains.

It seems likely that we will be able to harvest thousands of genomes
from metagenomic samples. The number of potentially useful samples is
growing exponentially, the desire to gain genomes for unculturable
organisms is growing, and our ability to extract reconstructed genomes
is improving. I believe that the quality produced by current algorithms
has reached the point where it is "good enough". Further improvements
will inevitably increase the fraction of bins that can be salvaged.
