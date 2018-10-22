.. _cli-common-tasks:

Common Tasks With P3 Scripts
============================

In this tutorial, we will present examples of common tasks and show how
to accomplish them with P3 scripts.

How do I find a genome from an accession number or project ID?
--------------------------------------------------------------

Genomes in PATRIC are stored with four alternate IDs, any of which
can be used to search for the genomes.

#. ncbi\_project\_id. The NCBI project number
#. refseq\_project\_id. The REFSEQ project number
#. genbank\_accessions. The accession string from GENBANK
#. refseq\_accessions. The accession string from REFSEQ

The following commands all return the genome *Streptococcus mutans
UA159*.

.. code::

    p3-all-genomes --eq genbank_accessions,AE014133

.. code::

    p3-all-genomes --eq refseq_accessions,NC_004350

.. code::

    p3-all-genomes --eq ncbi_project_id,333

.. code::

    p3-all-genomes --eq refseq_project_id,57947

Because no attributes were specified, the output in each case is
solely the genome ID, a single output record in a single column.

.. code::

    genome.genome_id
    210007.7

How do I find a feature from an alternate feature ID?
-----------------------------------------------------

Features in PATRIC are stored with four alternate IDs, all of which
are indexed for fast retrieval.

#. gene. The common gene name (e.g. ``ciaR``). Not all features will
   have a common gene ID
#. gene\_id. The gene number
#. refseq\_locus\_tag. The locus tag from REFSEQ

The command :ref:`cli::p3-find-features` is used to retrieve features based
on an alternate ID. The alternate IDs are piped in through the
standard input. Note that in some cases (e.g. the field ``gene``),
there may be a lot of features with the same ID. The following pipes
return the ID and functional assignment using alternate IDs.

.. code::

    p3-echo coaA | p3-find-features --attr patric_id,product gene

.. code::

    id  feature.patric_id   feature.product
    coaA    fig|996634.5.peg.916    Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|944560.4.peg.377    Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992133.3.peg.4201   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992141.3.peg.4166   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992132.3.peg.4176   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992136.3.peg.3951   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992139.3.peg.4173   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992131.3.peg.3905   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992142.3.peg.3915   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992137.3.peg.4122   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992135.3.peg.3895   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|99287.12.peg.4355   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|996306.3.peg.645    Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992175.3.peg.3998   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992179.3.peg.3888   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992177.3.peg.4127   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992178.3.peg.4122   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992180.3.peg.4094   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992172.3.peg.3873   Pantothenate kinase (EC 2.7.1.33)
    coaA    fig|992181.3.peg.3864   Pantothenate kinase (EC 2.7.1.33)

.. code::

    p3-echo 1029377 | p3-find-features --attr patric_id,product gene_id

.. code::

    id  feature.patric_id   feature.product
    1029377 fig|210007.7.peg.1009   Pantothenate kinase (EC 2.7.1.33)

.. code::

    p3-echo 24379558 | p3-find-features --attr patric_id,product gi

.. code::

    id  feature.patric_id   feature.product
    24379558    fig|210007.7.peg.1009   Pantothenate kinase (EC 2.7.1.33)

.. code::

    p3-echo SMU.1126 | p3-find-features --attr patric_id,product refseq_locus_tag

.. code::

    id  feature.patric_id   feature.product
    SMU.1126    fig|210007.7.peg.1009   Pantothenate kinase (EC 2.7.1.33)

Given a genome ID, how do I find the name?
------------------------------------------

The genome name is in an attribute called *genome\_name*. You can
get it from the genome ID using :ref:`cli::p3-all-genomes` as shown here.

.. code::

    p3-all-genomes --eq genome_id,210007.7 --attr genome_name

.. code::

    genome.genome_id    genome.genome_name
    210007.7    Streptococcus mutans UA159

Alternatively, you can use :ref:`cli::p3-get-genome-data` and use
:ref:`cli::p3-echo` to pipe in the ID.

.. code::

    p3-echo 210007.7 | p3-get-genome-data --attr genome_name

.. code::

    id  genome.genome_name
    210007.7    Streptococcus mutans UA159

Given a feature ID, how do I find the amino acid sequence?
----------------------------------------------------------

The amino acid sequence is in the attribute *aa\_sequence*. You use
:ref:`cli::p3-get-feature-data` to access it.

.. code::

    p3-echo "fig|210007.7.peg.1009" | p3-get-feature-data --attr aa_sequence

.. code::

    id  feature.aa_sequence
    fig|210007.7.peg.1009   MANEFINFEKISRKTWQHLHQESQPPLNENELNSIKSLNDRISIKDVTDIYLPLISLIQIYKKSQENLSFSKSIFLQKNISNRPFIIGVSGSVAVGKSTTSRLLQLLLARTFKDSSVELMTTDGFLYPNAVLSSRHMLNKKGFPESYDMERLLDFLDTIKNGQSAEIPVYSHEIYDIVPNKSQIIEVPDFLIIEGINVFQNPQNNRLYMSDFFDFSIYIDADSDYIENWYLERFATLLDLAKNDKQNYYNRFLKLGEKGALDFARDIWKDINLVNLEKYIEPTRSRAELILHKTKNHKIDEIYLKK

How do I find out how many genomes have an identical protein to a given feature?
--------------------------------------------------------------------------------

The individual protein sequences are not indexed, but the PATRIC
database contains an MD5 signature for each protein that is indexed,
in the feature attribute *aa\_sequence\_md5*. The following pipe
finds out how many times the protein sequence for
*fig\|210007.7.peg.1009* occurs in the database.

.. code::

    p3-echo "fig|210007.7.peg.1009" | p3-get-feature-data --attr aa_sequence_md5 | p3-find-features aa_sequence_md5 --count

.. code::

    id      feature.aa_sequence_md5 feature.count
    fig|210007.7.peg.1009   6400069a6f7f32515c3a584ade0588d0        150

The answer is 150, but that is not quite the question that was
asked. If the protein occurs more than once in a genome, then the
above count will be too high. To get the correct answer we need to
extract genome IDs and then count the number of distinct ones with
:ref:`cli::p3-count`.

.. code::

    p3-echo "fig|210007.7.peg.1009" | p3-get-feature-data --attr aa_sequence_md5 | p3-find-features aa_sequence_md5 --attr genome_id | p3-count genome_id

.. code::

    count
    149

How do I find all the genomes in a given genus?
-----------------------------------------------

The :ref:`cli::p3-all-genomes` script is used to do this. Simply filter on
the *genus* attribute.

.. code::

    p3-all-genomes --eq genus,Streptococcus --attr genome_id,genome_name

.. code::

    genome.genome_id    genome.genome_name
    1302.21 Streptococcus gordonii strain DD07
    1303.76 Streptococcus oralis strain DD05
    1303.77 Streptococcus oralis strain DD14
    1303.78 Streptococcus oralis strain DD15
    1303.79 Streptococcus oralis strain DD16
    1303.80 Streptococcus oralis strain DD20
    1303.81 Streptococcus oralis strain DD21
    1303.82 Streptococcus oralis strain DD27
    1303.83 Streptococcus oralis strain DD30
    1303.84 Streptococcus oralis strain DD24
    1303.86 Streptococcus oralis strain DD25
    1303.87 Streptococcus oralis strain DD17
    1318.28 Streptococcus parasanguinis strain DD19
    28037.233   Streptococcus mitis strain DD26
    28037.234   Streptococcus mitis strain DD28
    28037.238   Streptococcus mitis strain DD22

Given a feature ID, how do I find the features in the same protein family?
--------------------------------------------------------------------------

The family ID is in the *pgfam\_id* attribute, and we use
:ref:`cli::p3-get-family-features` with the ``--ftype=global`` to find the
other features.

.. code::

    p3-echo "fig|210007.7.peg.1009" | p3-get-feature-data --attr pgfam_id | p3-get-family-features --ne "patric_id,fig|210007.7" --ftype global --attr patric_id,genome_name,product

Note that we use the ``--ne`` operator to keep the original feature
from appearing in the output. Even so, the resulting file has over
67,000 results, the first few of which are shown below.

.. code::

    id  feature.pgfam_id    feature.patric_id   feature.genome_name feature.product
    fig|210007.7.peg.1009   PGF_00029921    fig|1341640.3.peg.2368  Yersinia sp. WP-930601  Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PGF_00029921    fig|1341642.3.peg.3368  Yersinia sp. WP-931205  Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PGF_00029921    fig|1344012.3.peg.2066  Tatumella sp. NML 06-3099   Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PGF_00029921    fig|984229.3.peg.2006   Salmonella enterica subsp. enterica serovar Enteritidis str. 653049 13-19   Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PGF_00029921    fig|984228.3.peg.4305   Salmonella enterica subsp. enterica serovar Enteritidis str. 648905 5-18    Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PGF_00029921    fig|984226.3.peg.4289   Salmonella enterica subsp. enterica serovar Enteritidis str. 648903 1-6 Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PGF_00029921    fig|984227.3.peg.3102   Salmonella enterica subsp. enterica serovar Enteritidis str. 648904 3-6 Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PGF_00029921    fig|984224.3.peg.642    Salmonella enterica subsp. enterica serovar Enteritidis str. 648901 39-2    Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PGF_00029921    fig|984225.3.peg.4221   Salmonella enterica subsp. enterica serovar Enteritidis str. 648902 6-8 Pantothenate kinase (EC 2.7.1.33)

Alternatively, you can use local protein families (*plfam\_id* for
the field name, and ``--ftype=local`` for the family type). This
will restrict the output to features for genomes in the same genus.

.. code::

    p3-echo "fig|210007.7.peg.1009" | p3-get-feature-data --attr plfam_id | p3-get-family-features --ne "patric_id,fig|210007.7" --ftype local --attr patric_id,genome_name,product

.. code::

    id  feature.plfam_id    feature.patric_id   feature.genome_name feature.product
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|1579339.3.peg.1420  Streptococcus sp. 449_SSPC  Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|511691.3.peg.905    Streptococcus mutans NN2025 Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|1404260.3.peg.1014  Streptococcus mutans PKUSS-LG01 Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|1403829.3.peg.1035  Streptococcus mutans PKUSS-HG01 Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|857136.3.peg.247    Streptococcus mutans A19    Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|857135.3.peg.392    Streptococcus mutans U138   Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|857134.3.peg.201    Streptococcus mutans G123   Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|857133.3.peg.623    Streptococcus mutans M21    Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|857132.3.peg.561    Streptococcus mutans T4 Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|857138.3.peg.734    Streptococcus mutans N29    Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|857137.3.peg.82 Streptococcus mutans NMT4863    Pantothenate kinase (EC 2.7.1.33)
    fig|210007.7.peg.1009   PLF_1301_00006228   fig|1313.8640.peg.2062  Streptococcus pneumoniae strain B16827  Pantothenate kinase (EC 2.7.1.33)

How do I find a gene by name in a particular genome?
----------------------------------------------------

Here you want to use :ref:`cli::p3-find-features` with a genome\_id filter.

.. code::

    p3-echo coaA | p3-find-features --attr patric_id,product --eq genome_id,210007.7 gene

.. code::

    id  feature.patric_id   feature.product
    coaA    fig|210007.7.peg.1009   Pantothenate kinase (EC 2.7.1.33)

