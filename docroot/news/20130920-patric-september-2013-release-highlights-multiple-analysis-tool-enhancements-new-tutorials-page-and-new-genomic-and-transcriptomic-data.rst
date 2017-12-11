=========================================================================================================================================
PATRIC September 2013 Release Highlights Multiple Analysis Tool Enhancements, New Tutorials Page, and New Genomic and Transcriptomic Data
=========================================================================================================================================


:Date:   2013-09-20T13:01:33+00:00

**Website Updates**
===================

***New Pathogen Interaction Gateway (PIG) for Protein-Protein
Interactions***

The `Pathogen Interaction Gateway
(PIG) <http://patricbrc.org/portal/portal/patric/HPITool?cType=taxon&cId=&dm=>`__
provides access to inter- and intra-species protein-protein interaction
(PPI) data for easy download or visualization.  PIG is available
currently as a Web application on both the Pathogen Portal (bacteria,
viruses, eukaryotic pathogens, hosts, and vectors) and PATRIC (bacteria
and hosts) websites.  Original PPI data are periodically downloaded from
public databases that include experimental data (predicted interactions
are not included in PIG), and are filtered for taxa of interest,
de-duplicated, and stored in local databases.  PIG allows users to
select custom sets of PPIs by taxon or keyword combinations, and
visualize the results in a coordinated interface that includes a
sortable list and interactive PPI node-edge graphs.  Multiple taxa can
be visualized simultaneously, enabling the detection of deeper
interaction motifs such as host proteins targeted by multiple pathogens,
or multiple classes of pathogen (bacterial, viral, eukaryotic), as well
as guilt-by-association clues to the function of unknown or hypothetical
proteins.\ ** **

***Genome Browser Enhancements, Featuring New Colors and the Ability to
Upload Your Own Data***

In this release, we have incorporated the latest version of JBrowse,
which provides enhanced interactivity and searching/filtering
mechanisms.  The browser now displays genomic features using a new color
scheme.  Different genomic feature types annotated by the same source
(such as PATRIC, RefSeq, and Legacy BRC) are now grouped as a single
track, using different shades of the same color to represent different
feature types.  Now, users can also upload their own annotations or gene
lists as GFF3 files and view them as tracks on the genome browser.  In
addition, users can also upload and view their RNA-Seq, ChiP-Seq, or SNP
data as tracks in the genome browser using BigWig or BAM file formats.
The latest genome browser for Mycobacterium tuberculosis H37Rv can be
viewed
`here <http://patricbrc.org/portal/portal/patric/GenomeBrowser?cType=genome&cId=87468&loc=0..10000&tracks=DNA,PATRICGenes,RefSeqGenes>`__.

***Enhanced Compare Region Viewer***

The Compare Region Viewer now uses the latest version of JBrowse and a
new, more vibrant color scheme.  In addition, genomes displayed in the
Compare Region Viewer can be filtered and sorted based on key genome
metadata attributes, such as isolation country, host, disease,
collection date, and completion date.  Here is an example of the
`Compare Region Viewer for Rv2429
gene <http://patricbrc.org/portal/portal/patric/CompareRegionViewer?cType=feature&cId=18153995&tracks=&regions=5&window=10000&loc=1..10000>`__
from the Mycobacterium tuberculosis H37Rv genome.

***New Transcriptomics Data Search and Display***

Improvements to transcriptomics data related functionality include
ability to search for transcriptomics experiments using Global Search
and a new Landing Page for transcriptomics experiments, showing
available metadata and curated comparisons for a single experiment.
 Here is an example of the transcriptomics experiment page for the
latest Burkholderia pseudomallei dataset,
`GSE43205 <http://patricbrc.org/portal/portal/patric/SingleExperiment?cType=taxon&cId=2&eid=1191081>`__,
added to PATRIC.

***Performance Improvements to Protein Family Sorter and Transcriptomics
Gene List***

The performance of the Protein Family Sorter and Transcriptomics Gene
List pages have been improved to make them load faster and compare
larger numbers of genomes and transcriptomics experiments, respectively.

***New Tools and Tutorial Landing Pages***

Two new help pages have been developed:  The `Tutorials Landing
Page <http://patricbrc.org/portal/portal/patric/Tutorials>`__ features
all available video tutorials, workflows, and step-by-step PDF tutorials
showcasing how to use PATRIC data and analysis tools.  The `Tools
Landing Page <http://patricbrc.org/portal/portal/patric/Tools>`__
provides descriptive summaries and links to all the tools available on
PATRIC.

**New Genomes and Annotations**
===============================

In the September 2013 data release, `2911 new genomes have been
added <ftp://ftp.patricbrc.org/patric2/RELEASE_NOTES/Sept2013/genomes_added>`__
to PATRIC, `2887 new genomes have been annotated using
RAST <ftp://ftp.patricbrc.org/patric2/RELEASE_NOTES/Sept2013/new_genomes_annotated>`__,
`16 genomes have been
updated <ftp://ftp.patricbrc.org/patric2/RELEASE_NOTES/Sept2013/genomes_updated>`__
and `2 genomes have been
deleted <ftp://ftp.patricbrc.org/patric2/RELEASE_NOTES/Sept2013/genomes_deleted>`__.

A summary of the genomes available on the PATRIC website through
September, 2013 is provided in the table below:

.. raw:: html

   <div align="center">

.. raw:: html

   <table width="74%" border="1" cellspacing="0" cellpadding="0">

.. raw:: html

   <tr>

.. raw:: html

   <td width="69%">

.. raw:: html

   </td>

.. raw:: html

   <td width="16%">

.. raw:: html

   <p align="right">

PATRIC

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="13%">

.. raw:: html

   <p align="right">

RefSeq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="69%">

Number of genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="16%">

.. raw:: html

   <p align="right">

11787

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="13%">

.. raw:: html

   <p align="right">

8964

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="69%">

Number of Complete genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="16%">

.. raw:: html

   <p align="right">

2260

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="13%">

.. raw:: html

   <p align="right">

2204

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="69%">

Number of WGS genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="16%">

.. raw:: html

   <p align="right">

9523

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="13%">

.. raw:: html

   <p align="right">

6361

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="69%">

Number of Plasmid only genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="16%">

.. raw:: html

   <p align="right">

4

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="13%">

.. raw:: html

   <p align="right">

399

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </table>

.. raw:: html

   </div>

***Featured: 42 New Brucella Genomes and 270 new Mycobacterium bovis
Genomes from USDA***

This data release features `42 new Brucella genomes (in addition to 106
genomes released in
May) <http://test.patricbrc.org/portal/portal/patric/GenomeList?cType=taxon&cId=234&kw=USDA+AND+2013>`__
and `270 new Mycobacterium bovis
genomes <http://test.patricbrc.org/portal/portal/patric/GenomeList?cType=taxon&cId=1763&kw=USDA+AND+2013-09-01>`__
that are available exclusively at PATRIC. These genomes were sequenced
by USDA and, subsequently, assembled and annotated by PATRIC using RAST.

***Genome Metadata***

In addition to manual curation of metadata for new genomes, we have also
incorporated additional metadata for 712 genomes using metadata we
received from NIAID-funded Genome Sequencing Centers.

**New Transcriptomics Datasets**
================================

In the September data release, 20 new GEO experiments have been curated
and incorporated into PATRIC.  Below is the summary of the new
experiments and curated comparisons added to PATRIC since June 2013.

.. raw:: html

   <div align="center">

.. raw:: html

   <table width="253" border="0" cellspacing="0" cellpadding="0">

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Organisms

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

Experiments

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

Comparisons

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Bdellovibrio

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Burkholderia

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

82

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Desulfovibrio

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

9

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Fusobacterium

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

3

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Myxococcus

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

75

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Pasteurella

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

103

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Pseudomonas

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

13

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

79

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Rhodobacter

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

8

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Rhodopseudomonas

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

6

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="102">

Zymomonas

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="73">

.. raw:: html

   <p align="right">

1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="bottom" nowrap="nowrap" width="78">

.. raw:: html

   <p align="right">

4

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </table>

.. raw:: html

   </div>
