:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/20170930-patric-september-2017-data-release.rst

PATRIC September 2017 Data Release
==================================

.. feed-entry::
   :date: 2017-09-30

In this release, PATRIC has added >7,500 new genomes and associated metadata, bringing the total number of genomes in
PATRIC to over 116,000. This release features 1,668 Klebsiella pneumoniae genomes, which are clinical isolates from
Houston Methodist Hospital System and contain AMR panel data.

.. cut::

Data Updates:
-------------

New Genomes and Metadata
~~~~~~~~~~~~~~~~~~~~~~~~

In this release, PATRIC has added >7,500 new genomes and associated metadata, bringing the total number of genomes in
PATRIC to over 116,000. The full list of available microbial and host genomes can be accessed `here
<https://www.patricbrc.org/view/GenomeList/?or(keyword(Bacteria),keyword(Archaea),keyword(Eukaryota))#view_tab=genomes>`__.

This release features 1,668 Klebsiella pneumoniae genomes, which are clinical isolates from Houston Methodist Hospital
System and contain AMR panel data. These genomes and related AMR data are exclusively available in PATRIC and were used
in constructing new `AMR phenotype prediction <http://mbio.asm.org/content/8/3/e00489-17.short>`__ and `Minimum
Inhibitory Concentration (MIC) prediction <https://www.biorxiv.org/content/early/2017/09/25/193797>`__ classifiers in
PATRIC.

Annotation and Protein Family Updates
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

As part of this release, we have updated protein functions and protein families for all public genomes in PATRIC. This
is done periodically (usually every four months) to incorporate the latest annotations from the manual curation of
underlying subsystems and AMR genes. The genus-specific and cross-genera protein families are also updated to increase
the coverage for novel proteins and novel genera added in the database since last update. The new protein annotations
and protein families are also deployed in the annotation pipeline. Hence, any new genomes annotated using the PATRIC
Annotation Service will receive the latest annotations.

Specialty Gene Updates
~~~~~~~~~~~~~~~~~~~~~~

All reference gene databases used for Specialty Gene Annotation have been updated to incorporate the latest data from
the original source databases, including CARD, VFDB, Victors, DrugBank and TTD. In addition, we have added two new
reference databases: AMR genes from NCBI’s NDARO database and transporter genes from TCDB. The specialty gene
annotations for all public genomes in PATRIC have been updated and the new reference databases are deployed as part of
the PATRIC Annotation Service.

Website Updates:
----------------

The website updates include minor enhancements and bug fixes identified from recent PATRIC workshops as well as direct
user feedback, including the following:

* Streaming of results from the Variation, RNA-seq, and Tn-seq services (i.e. BAM and VCF files) to the Genome Browser directly from the jobs result page.
* Ability to provide SRA Run Accession as input to the Assembly Service, without uploading the read files.
* Improved performance and load times for the Protein Family Sorter and other pages.
* Enhancements to the workspace data management, including efficient copying and moving job results.

.. spelling::
   pneumoniae