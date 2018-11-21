.. _gui-tasks:

Common Tasks Using the Web Interface
====================================

In this tutorial, we will present examples of common tasks and show how
to accomplish them using the PATRIC Web Interface.  To keep this page
manageable, we link to instructions on separate pages.

Working with Sequences
----------------------


Assemble a Set of Reads into Contigs
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

PATRIC provides an assembly service that allows you to choose between multiple assemblers,
using either single-read libraries, paired-end reads, or reads stored online in the
`NCBI Sequence Read Archive <https://www.ncbi.nlm.nih.gov/sra/>`_.  We have an
:doc:`introductory tutorial </tutorial/genome_assembly/assembly>` and
a :doc:`more detailed guide </user_guides/services/genome_assembly_service>`.

Create an Annotated Genome from a set of contigs and Estimate its Quality
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

PATRIC provides an annotation service that constructs a private genome from
contigs and produces a quality report.  See :doc:`/tutorial/genome_annotation/annotation`
for instructions on submitting the contigs, and :doc:`/tutorial/genome_quality_report/genome_quality_report`
to read the quality report.

Extract as Many Complete Genomes as Possible from a Meta-Genomic Sample
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The :doc:`/user_guides/services/metagenome_binning_service` provides this function.  For a tutorial,
see :doc:`/tutorial/metagenomic_binning/metagenomic_binning`.

Annotate a New Genome and Compare it to Similar Genomes in PATRIC
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
This combines several of the tasks listed elsewhere on this page.  The
Comprehensive Genome Analysis service takes either reads or contigs and
creates a private genome integrated into the PATRIC database. It also
creates a web page describing the genome and places it into a phylogenetic
tree.  There is a tutorial on how to use this service
`here </tutorial/comprehensive-genome-analysis/comprehensive-genome-analysis>`_.
In :doc:`/tutorial/comprehensive-genome-analysis/cga-results` we show how to
look at the results, find the closest genomes, and compare the protein families.


Working with Taxonomic Groups
-----------------------------

Find Representative Genomes for a Taxon
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

NCBI identifies
`Reference and Representative genomes for each clade and species <https://www.ncbi.nlm.nih.gov/refseq/about/prokaryotes/#representative_genomes>`_.
To these lists, PATRIC adds UniProt reference genomes, and additional genomes selected by manual
curation.  Because of their high quality, they are a useful subset for doing certain types of
analysis.

For the procedure to list the genomes in a taxonomic grouping, see :doc:`/tutorial/searching_and_sorting/genomes_by_taxonomy`.
Instructions for isolating the Reference and Representative genomes are given on the same page under the heading
:ref:`rep-ref-taxon-section`.

Find Genomes in a Taxon with Specific Attributes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For the procedure to list the genomes in a taxonomic grouping, see :doc:`/tutorial/searching_and_sorting/genomes_by_taxonomy`.
Instructions for filtering the list are given on the same page under the heading
:ref:`taxon-exotic-filtering-section`.


Working with Genomes
--------------------

Find the Roles Present in a Genome
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This is described at :doc:`tutorial/searching_and_sorting/features_with_roles`.

Compare the Proteomes for a Set of Genomes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This is described at :doc:`/tutorial/proteome_comparison/proteome_comparison`.

Visually Compare the Protein Families in a Set of Genomes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This is described at :doc:`/tutorial/protein_family_sorter/protein_family_sorter`.  A description of
the output and how to manipulate it can be found `here </user_guides/organisms_taxon/protein_families.html#protein-family-sorter-heatmap>`_

Working with Alignments and Trees
---------------------------------

Create a Phylogenetic Tree from a DNA Alignment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Phillipe's task: Given a DNA alignment, compute a phylogenetic tree.

Create a Phylogenetic Tree from a Protein Alignment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Phillipe's task: Given a protein alignment, compute a phylogenetic tree.

Given an alignment/tree and a separate sequence, insert the new sequence
into the alignment/tree.


Working with Protein Families
-----------------------------

List the Features in a Protein Family and the Genomes Containing Them
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Phillipe's task: Given a protein family get the (genome,peg) tuples for the family.

Find the Function of a Protein Family
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Phillipe's task: Given a protein family get the function of the family.



Working with Features
---------------------


Find the Sequence, Translation, and Other Known Attributes of a Gene
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Phillipe's task: Given a peg, get the known attributes of the peg (including sequence
and translation).

Find the Upstream Region of a Gene
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Phillipe's task: Given a peg, get its upstream region.



Compute the CDD Domains for a Gene
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This service is no longer available in PATRIC. A request is pending.


Create an Alignment and the Associated Phylogenetic Tree from a Set of Features
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This is described in :doc:`/tutorial/alignments/multiple_sequence_alignment`.

Find the Papers Relating to a Specific Feature
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Bruce text

Find the Subsystems Supported by a Set of Functional Roles
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Bruce text

Determine the Evidence of Quality for a Genome
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Phillipe's task: What does the "evidence of quality" for a genome mean?

Find the Closest N Genomes to a Particular Genome
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Phillipe's task: Given a genome get the closest N genomes.

