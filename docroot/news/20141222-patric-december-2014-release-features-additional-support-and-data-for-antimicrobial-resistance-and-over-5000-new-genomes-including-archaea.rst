============================================================================================================================================
PATRIC December 2014 Release Features Additional Support and Data for Antimicrobial Resistance and over 5,000 New Genomes, Including Archaea
============================================================================================================================================


:date:   2014-12-22T16:28:05+00:00

This December Release sets the stage for new functionality and data in
PATRIC. In 2015, our primary goals are as follows:

-  Revamp PATRIC infrastructure to support the hundreds of thousands of
   prokaryotic genomes that will become available over the next five
   years, providing real-time integration and release of data.
-  Support end-to-end analysis of prokaryotic genomes to allow
   researchers to upload their own sequencing reads to PATRIC, assemble
   genomes and annotate them using RAST. Researchers will be able to
   analyze their private genomes using the tools available at PATRIC,
   and then they can make their genomes publicly available at PATRIC if
   desired.
-  Incorporate all published Archaea genomes and selected Eukaryotic
   host genomes.
-  Integrate existing data analysis tools from the RAST/SEED systems
   into PATRIC.
-  Incorporate genome metadata related to antibiotic resistance and
   provide enhanced search and analysis tools to allow researchers to
   easily examine this data.
-  Enhance the user experience by providing improved functionality for
   searching and analyzing data in the PATRIC resource.

In order to enable these functions and other enhancements, we will make
some changes to the existing PATRIC system and ask for your patience and
support as we go through this period of transition.

Antimicrobial Resistance and other Clinical Metadata
====================================================

In this release, we have started to incorporate antimicrobial resistance
(AMR) information at the genome level. This is a first step, as the
coverage and the search and analysis capabilities will become richer in
future releases. This release includes curated metadata from `nine
sequencing
projects <http://enews.patricbrc.org/niaid-antimicrobial-resistance-sequencing-projects/>`__
from the NIAID-funded Genomic Centers for Infectious Diseases. This data
covers 1247 genomes from 10 genera, including 53 antibiotics and 4
chemicals. We have also enhanced PATRIC support for the clinical
metadata that is frequently generated in projects which sequence many
clinical isolates to study AMR.

In this release, support for AMR metadata includes:

-  **Antimicrobial Resistance** metadata field. This field shows genomes
   that have been specifically tested against certain antibiotics and
   the resulting phenotype from that test. Note that a genome can have
   multiple antibiotic phenotypes, such as being resistant to one drug
   and susceptible to another. The values included in this field are:

   -  ‘Resistant’ (984 genomes)
   -  ‘Susceptible’ (687 genomes)
   -  ‘Intermediate’ (239 genomes)

-  **Antimicrobial Resistance Evidence** metadata field. Some of the
   genomes included in PATRIC have a specific phenotype that has been
   assigned, such as MRSA, and some of the genomes have been screened by
   broad, antimicrobial resistant panels (AMR panels). We have created a
   new field that identifies which metadata available on the PATRIC
   website contains the evidence supporting the resistance category
   assigned.

   -  ‘Phenotype’ (607 genomes). Genomes in this category were assigned
      their resistance category based on phenotype information provided
      by the sequencing center, for instance MRSA or MSSA. This
      phenotype data is available at PATRIC as well.
   -  ‘AMR Panel’ (588 genomes). Some genomes have been tested against a
      panel of antibiotics, with the results of the screening reported
      in a table using either a specific designation (such as
      ‘Susceptible,’ ‘Resistant,’ or ‘Intermediate’), or the minimum
      inhibitory concentration (MIC). For genomes in this category, the
      panel data is available for download. In future releases, this
      data will be more fully integrated on the PATRIC website.
   -  ‘Comment’ (52 genomes). The basis for the resistance category for
      these genomes can be found in the comment metadata field. This
      information may have come from the comment field at GenBank, or in
      a comment field from data provided by the sequencing center or
      their sample provider. In some cases, the comment has been
      provided by literature-based curation by the PATRIC team; in these
      cases, a link to the corresponding publication is also available.

The Antimicrobial Resistance metadata field and the Antimicrobial
Resistance Evidence metadata field are now available as filterable
facets on the Genome list pages, which allows researchers to sort on the
terms ‘Susceptible’, ‘Resistant’ or ‘Intermediate’ to locate the genomes
tagged with that information. In addition, the researcher can filter on
the source of the information, which provides the ability, for example,
to only use genomes that have complete AMR panel information and exclude
genomes where there is only a comment.

This release also adds enhanced support to allow storing and retrieving
some clinical metadata that is available for only some of the genomes
available at PATRIC. This includes new typing methods that are specific
to a small number of genomes (such as spa type or wzi type), but are
still important to researchers. This data is stored as a key-value pair
so that researchers using Global Search can find genomes that contain
any data for that field (e.g., search for ‘wzi’) or for genomes with
specific values for that field (e.g., search for ‘wzi:29’)

Researchers can now use the Show/Hide capability on Genome lists to
expose or hide the new metadata fields. The information is also
available on each Genome Summary page by selecting clicking on the
Summary information. When a list of genomes is downloaded, all of the
new metadata fields are also included in the list of metadata available.

Changes in the Identifier Scheme
================================

In order to prepare PATRIC for the continuing rapid growth of genomes
and other data types over next five years, and to achieve tighter
integration with the RAST annotation service, we have made the following
changes in the PATRIC identifier scheme.

-  **Archived identifiers**. For all genomes included in PATRIC up to
   this point, the following identifiers have been archived and will
   continue to be available as alternate identifiers. However, new
   genomes added in PATRIC, beginning with this release, will not be
   assigned these identifiers.

   -  Genome_info_id or gid. This numeric identifier used to uniquely
      identify any genome in PATRIC. Old identifiers for genomes will be
      archived as “p2_genome_id.”
   -  Feature_info_id or fid. These are numeric identifiers that are
      used to uniquely identify a genomic feature, such as a gene, CDS,
      or RNAs. Old identifiers for features will be archived as
      “p2_feature_id.”
   -  VBI Locus Tag. Previously, we provided locus tags for genes, CDSs,
      and RNAs that start with a VBI prefix; this practice will be
      discontinued. The old VBI prefix locus tags will be archived as
      “Alt_locus_tag.”

-  **New Identifiers**.

   -  Genome_ID. A numeric identifier scheme adopted from RAST/SEED
      genome ids in the form taxon_id.version (i.e., 83332.12) will be
      assigned to every genome in PATRIC. This identifier will be used
      in both the PATRIC and RAST systems.
   -  PATRIC_ID. A new identifier, also adopted from RAST/SEED, will be
      assigned to genomic features annotated using RAST. This identifier
      scheme is in the form fig|83332.12.peg.1. This will replace the
      VBI locus tag.
   -  Feature_ID. PATRIC will now include a new identifier that is
      composed of annotation source, genome_id, sequence_accession,
      feature_type, start, end, and strand. For example:

      RefSeq.83332.12.NC_000962.CDS.1.1524.fwd

      PATRIC.83332.12.NC_000962.CDS.34.1524.fwd

      The Feature_ID will not be displayed prominently on the website,
      but will be used to uniquely identify features in the database and
      generate mappings. Other more popular identifiers such as RefSeq
      locus_tag and the new PATRIC_ID will be displayed in tables and
      download files.

Upcoming Changes to the FTP site
================================

In order to support multiple genomes that have the same name, we will be
reorganizing the PATRIC FTP file download area. This is a work in
progress and we hope to release these genomes on the FTP site by the end
of January 2015.

Upcoming Updates to BLAST
=========================

We are currently working to improve the BLAST search available at
PATRIC, both in terms of its usability and performance. As of this
release, the new genomes have not been added to the BLAST search. New
genomes will be added to BLAST search when the improved version of BLAST
is released early in 2015.

New Genomes and Annotations
===========================

Archaeal Genomes
----------------

The PATRIC December Release includes 421 Archaea genomes with both
GenBank and RAST annotations. Researchers can now analyze these genomes
using all the tools available in PATRIC. We will routinely pick up new
Archaea genomes available at GenBank and make them available at PATRIC.

New Bacterial Genomes
---------------------

In this release, 4942 new bacterial genomes have been added to PATRIC.

Removal of Plasmid Only / Deprecated / Obsolete / Erroneous genomes
-------------------------------------------------------------------

In this release, we have removed 482 bacterial genomes from PATRIC. Many
of these genomes were only plasmids and lacked chromosomal sequences,
and size limitations meant that they could not be annotated by RAST.
Other genomes that were removed included genomes that were identified as
obsolete at GenBank, or that had multiple versions of the same genome
grouped together. Removing these genomes was a necessary part of
database clean up. If any of these genomes or their corresponding genes
were included in your workspace groups, they are no longer visible. If
you need this data, please contact us at patric@vbi.vt.edu and we will
work with you to retrieve the information you need.
