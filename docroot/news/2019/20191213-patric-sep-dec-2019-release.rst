:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/2019/20190731-patric-july-2019-release.rst

PATRIC July 2019 Data and Website Release
==============================================

.. feed-entry::
   :date: 2019-07-31

This PATRIC release includes a new Fastq Utilities Service and over 24,500 new microbial genomes.  


.. cut::


Data Updates:
--------------

**New Genomes**

In this release, PATRIC has added 24,542 new genomes bringing the total number of genomes and plasmids in PATRIC to over 250,000. To support the rapidly growth of number of genomes, the PATRIC backend database has been converted from SolrCloud, which greatly increases storage capacity as well as improving performance. The full list of available microbial and host genomes can be accessed `here
<https://www.patricbrc.org/view/GenomeList/?or(keyword(Bacteria),keyword(Archaea),keyword(Eukaryota))#view_tab=genomes>`__.


New Website Features:
----------------------
The new **Fastq Utilities Service** provides the capability for aligning, measuring base call quality, and trimming fastq read files to estimate quality. Fastq reads (paired-or single-end, long or short, zipped or not), as well as Sequence Read Archive accession numbers are supported. The three components (trim, fastqc and align) can be used independently, or in any combination. The `Fastq Utilities Service <https://www.patricbrc.org/app/FastqUtil>`_ is available from the Services top menu.
