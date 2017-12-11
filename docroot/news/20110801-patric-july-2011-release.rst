:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/20110801-patric-july-2011-release.rst

================================================================
PATRIC July 2011 Release Features Integration of Genome Metadata
================================================================

.. feed-entry::
   :date: 2011-08-01

**New Searches and Tools**
==========================

**Integration of Genome Metadata**

PATRIC has collected metadata associated with bacterial genomes from
multiple sources, such as NCBI’s BioProject database, GenBank records,
and the Human Microbiome Project.  Following the automated collection,
the metadata was manually curated for consistency and accuracy,
organized into a relational database, and integrated with the genomes
available in PATRIC.  This metadata provides useful information about a
genome, including genome status, isolation source, isolation country,
collection date, host organism, associated disease, and more. The
metadata is organized into the following broad categories:  organism
info, project info, sequence info, isolate info, host info, and
phenotype info.

Genome metadata can be accessed in multiple ways on the PATRIC website:

-  The improved Genome Finder allows users to locate genomes available
   in PATRIC by their associated metadata. A keyword search allows for
   the search across all available metadata fields, including the
   free-text comments. These search results are summarized by key
   metadata attributes, including genome status, isolation country, host
   name, disease, collection date, and completion date.  Progressive
   filtering of the results is also available. 
   http://patricbrc.org/portal/portal/patric/GenomeFinder?cType=taxon&cId=&dm\ =

-  A summary of key metadata attributes is provided on every Taxon
   Overview page.

.. raw:: html

   <p style="padding-left: 30px;">

For an example see: 
http://patricbrc.org/portal/portal/patric/Taxon?cType=taxon&cId=561

.. raw:: html

   </p>

-  Metadata is also available at the Genome List tab, present at all
   taxonomy levels.  Progressive filtering by key metadata attributes is
   provided.  The Genome List table allows users to choose any of the 61
   currently available metadata attributes and add them to the table as
   columns. In addition, users can also download all available genomes
   and associated metadata as a tab delimited or Excel file.  For an
   example see:

.. raw:: html

   <p style="padding-left: 30px;">

http://patricbrc.org/portal/portal/patric/GenomeList?cType=taxon&cId=561&dataSource=&displayMode=&pk=9379#key=9379&pS=20&aP=1&aT=0&cwG=false&cF=&gId=&gName=&gdir=ASC&gsort=genome_name&sdir=&ssort=

.. raw:: html

   </p>

-  All available metadata for an individual genome is located on the
   Genome Overview Page under Genome Summary.

.. raw:: html

   <p style="padding-left: 30px;">

http://patricbrc.org/portal/portal/patric/Genome?cType=genome&cId=200960

.. raw:: html

   </p>

To learn more about the genome metadata available at PATRIC, or how to
search for a genome by its available metadata, visit `Genome Metadata
FAQs <../../../../../faqs/genome-metadata-faqs/>`__ or `Genome Finder
FAQs <../../../../../faqs/genome-finder-faqs/>`__, respectively.

The collection and refinement of genome metadata is an ongoing task.
Future plans include integrating the genome metadata with various
analysis tools available on the PATRIC website.

**Data Download in GFF Format**

PATRIC annotations are now available for download as GFF files, which
can be accessed via the Downloads tab at the top of any PATRIC page.
 Alternatively, GFF files can be accessed by clicking “Download genome
data” in the upper-right of any PATRIC Genome Overview page.  For an
example, see:

http://brcdownloads.vbi.vt.edu/patric2/genomes/Escherichia_coli_O104-H4_str_LB226692/Escherichia_coli_O104-H4_str_LB226692.PATRIC.gff

**Genomes and Annotations**
===========================

Since the June release, `756 new
genomes <http://brcdownloads.vbi.vt.edu/patric2/genomes/RELEASE_NOTES/genomes_added>`__
have been added to PATRIC.  Many of them are draft assemblies available
in GenBank but not in RefSeq. In addition, `62 genomes have been
updated <http://brcdownloads.vbi.vt.edu/patric2/genomes/RELEASE_NOTES/genomes_updated>`__
or replaced with their newest versions. In total, 749 new genomes have
been annotated using RAST.

A summary of the genomes available on the PATRIC website through July,
2011 is provided in the table below:

.. raw:: html

   <table width="100%" border="0" cellspacing="0" cellpadding="0">

.. raw:: html

   <tr>

.. raw:: html

   <td>

.. raw:: html

   <table width="434" border="0" cellspacing="0" cellpadding="0">

.. raw:: html

   <tr>

.. raw:: html

   <td width="39%">

.. raw:: html

   </td>

.. raw:: html

   <td width="19%">

PATRIC

.. raw:: html

   </td>

.. raw:: html

   <td width="22%">

Legacy BRC

.. raw:: html

   </td>

.. raw:: html

   <td width="18%">

RefSeq

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="39%">

Number of genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="19%">

3535

.. raw:: html

   </td>

.. raw:: html

   <td width="22%">

337

.. raw:: html

   </td>

.. raw:: html

   <td width="18%">

3685

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="39%">

Number of Complete genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="19%">

1491

.. raw:: html

   </td>

.. raw:: html

   <td width="22%">

237

.. raw:: html

   </td>

.. raw:: html

   <td width="18%">

1488

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="39%">

Number of WGS genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="19%">

2044

.. raw:: html

   </td>

.. raw:: html

   <td width="22%">

96

.. raw:: html

   </td>

.. raw:: html

   <td width="18%">

1800

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="39%">

Number of Plasmid only genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="19%">

.. raw:: html

   </td>

.. raw:: html

   <td width="22%">

4

.. raw:: html

   </td>

.. raw:: html

   <td width="18%">

397

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </table>

.. raw:: html

   <p>

 

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

.. raw:: html

   <p>

To view this Sequence Summary along with Genomic and Protein Feature
Summaries, please
visit: http://patricbrc.org/portal/portal/patric/Taxon?cType=taxon&cId=2

.. raw:: html

   </p>
