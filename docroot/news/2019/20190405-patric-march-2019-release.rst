:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/2019/2019040507-patric-march-2019-release.rst

PATRIC March 2019 Data and Website Release
==============================================

.. feed-entry::
   :date: 2019-04-05

This PATRIC release includes a new Metagenome Taxonomic Classification Service; a new Metagenomic Read Mapping Service; a new Codon Tree option for the Phylogenetic Tree Building Service; and over XX,XXX new microbial genomes.  



.. cut::


Data Updates:
--------------

**New Genomes**

In this release, PATRIC has added 18,250 new genomes with AMR panel data added since January release, which includes 10,000 genomes from MTB Cryptic consortium and 5000 genomes from SRA with antibiogram data. All of these genomes were assembled from reads in SRA. We also updated MLST reference database and MLST assignments for all public genomes and standardized host names for all public genomes to support development of new machine learning models to predict host specificity. The total number of genomes and plasmids in PATRIC is now over 230,000. The full list of available microbial and host genomes can be accessed `here
<https://www.patricbrc.org/view/GenomeList/?or(keyword(Bacteria),keyword(Archaea),keyword(Eukaryota))#view_tab=genomes>`__.


New Website Features:
----------------------
The new **Metagenome Taxonomic Classification Service** accepts reads or contigs from sequencing of a metagenomic sample and uses Kraken 2 to assign the reads to taxonomic bins, providing an initial profile of the possible constituent organisms present in the sample. The `Taxonomic Classification Service <https://patricbrc.org/app/TaxonomicClassification>`_ is available from the Services top menu.

The new **Metagenomic Read Mapping Service** uses KMA to align reads against antibiotic resistance genes and virulence factors in PATRIC. The `Metagenomic Read Mapping Service <https://patricbrc.org/app/MetagenomicReadMapping>`_ is available from the Services top menu.

The **Phylogenetic Tree Builiding Service** now includes a faster **Codon Tree** option that utilizes PATRIC PGFams as homology groups and analyzes aligned proteins and coding DNA from single-copy genes using the program RAxML. Up to 100 genomes can be analyzed. The `Phylogenetic Tree Building Service <https://patricbrc.org/app/PhylogeneticTree>`_ is available from the Services top menu.
