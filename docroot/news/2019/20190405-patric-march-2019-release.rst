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

In this release, PATRIC has added over XX,XXX new genomes and associated metadata, bringing the total number of genomes and plasmids to over 230,000. The full list of available microbial and host genomes can be accessed `here
<https://www.patricbrc.org/view/GenomeList/?or(keyword(Bacteria),keyword(Archaea),keyword(Eukaryota))#view_tab=genomes>`__.


New Website Features:
----------------------
The new **Metagenome Taxonomic Classification Service** accepts reads or contigs from sequencing of a metagenomic sample and uses Kraken 2 to assign the reads to taxonomic bins, providing an initial profile of the possible constituent organisms present in the sample. The `Taxonomic Classification Service <https://patricbrc.org/app/TaxonomicClassification>`_ is available from the Services top menu.



The assembly component of the **Metagenomic Binning Service** has been migrated to a 1024-node cluster, enabling a 10-fold increase in the throughput of assembly-based binning jobs. The `Metagenomic Binning Service <https://patricbrc.org/app/MetagenomeBinning>`_ is available from the Services top menu.

The **RNA-Seq Analysis Service** now supports direct import of sequence data from SRA, alleviating the need to first download the data from SRA and then upload into the service. The `RNA-Seq Analysis Service <https://patricbrc.org/app/Rnaseq>`_ is available from the Services top menu. 

The **Tn-Seq Analysis Service** has been updated to use a new version of the TRANSIT software. The `Tn-Seq Analysis Service <https://patricbrc.org/app/Tnseq>`_ is available from the Services top menu.
