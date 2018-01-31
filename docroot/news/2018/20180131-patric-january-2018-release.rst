:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/2018/20180131-patric-january-2018-release.rst

PATRIC January 2018 Data and Website Release
==============================================

.. feed-entry::
   :date: 2018-01-31

In this release, PATRIC has added over 4,000 new genomes and associated metadata, bringing the total number of genomes and plasmids in PATRIC to over 150,000. This release also features a new Metagenomic Binning Service that allows users to assemble and annotate high-quality microbial genomes directly from metagenomic reads.
.. cut::


Data Updates:
--------------

**New Genomes and Metadata**

In this release, PATRIC has added over 4000 new genomes and associated metadata, along with a new plasmid database (described below) bringing the total number of genomes and plasmids in PATRIC to over 150,000. The full list of available microbial and host genomes can be accessed `here
<https://www.patricbrc.org/view/GenomeList/?or(keyword(Bacteria),keyword(Archaea),keyword(Eukaryota))#view_tab=genomes>`__.

This release features additional AMR for 988 genomes already in PATRIC, curated from publications.  It also includes over 2000 new genomes from published AMR studies that have been assembled from SRA and incorporated into PATRIC, along with the associated AMR metadata.

**New Plasmid Database**

As part of this release, we have added a new plasmid database with over 10,000 plasmid sequences, which are not associated with sequenced genomes in PATRIC. All plasmids are consistently annotated using the PATRIC Annotation Service and can be compared using various comparative genomics tools in PATRIC. Plasmids can be found in PATRIC by filtering any list of genomes in PATRIC where the Genome Status field is "Plasmid," for example, as shown `here
<https://www.patricbrc.org/view/GenomeList/?and(or(eq(genome_status,%22Plasmid%22)),eq(public,%22true%22))#view_tab=genomes`__.


New Website Features:
--------------

**Metagenomic Binning Service**

This release includes a new Metagenomic Binning Service that allows users to assemble and annotate high-quality microbial genomes directly from metagenomic reads.  The service is available at `Metagenome Binning Service <https://www.patricbrc.org/app/MetagenomeBinning>`__. Note that you must be logged in to PATRIC to use the service. There is also an associated tutorial describing how to use the service: `Using the PATRIC Metagenomics Binning Service  <https://docs.patricbrc.org/tutorial/metagenomic_binning/metagenomic_binning.html>`__.



