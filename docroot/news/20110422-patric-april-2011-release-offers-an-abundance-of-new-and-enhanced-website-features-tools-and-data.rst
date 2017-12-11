===================================================================================================
PATRIC April 2011 Release Offers an Abundance of New and Enhanced Website Features, Tools, and Data
===================================================================================================

:Author: patricwpadmin
:Date:   2011-04-22T20:24:43+00:00

**Website Enhancements**
========================

**Enhanced Protein Family Sorter Can Now Sort Based on Gene Order**

-  The Heatmap Viewer associated with the protein family sorter now
   allows one to choose a reference genome to act as an anchor and then
   sort all the protein families based on the gene order in that genome.
   This functionality allows the user to quickly identify groups of
   contiguous genes present or absent in one or more of the selected
   genomes.  In addition, the user can quickly visualize areas of loss
   or gain of genomic segments across genomes that are closely or more
   distantly related.  Some of these areas may correspond to
   pathogenicity islands.

-  The color scheme of the Heatmap has been changed to improve visual
   field differentiation,

-  Advanced filters have been added that allow the user to search for
   perfect or non-perfect protein families and filter them by the number
   of members and/or genomes per protein family.

For an example, please visit the following page and click on the
“Heatmap” tab:

http://patricbrc.org/portal/portal/patric/FIGfamSorterB?cType=taxon&cId=1392&dm=result

**Improved Comparative Pathway Analysis with New Heatmap Viewer**

-  A new interactive feature that shows the presence or absence of EC
   numbers in pathways has been added.  This feature is in the form of a
   Heatmap Viewer and it allows users to see the presence or absence of
   individual EC numbers within a pathway, with the ability to make
   comparisons across a wide number of genomes.

-  In addition, the data supporting the Heatmap visualization, such as
   the individual locus tags or the presence/absence across genomes of
   interest, is available for download by users.

For an example, please visit the following page and click on the
“Heatmap” tab:

http://patricbrc.org/portal/portal/patric/CompPathwayMap?cType=taxon&cId=234&map=00362&algorithm=PATRIC

**Save Your PATRIC Data With Our New User Registration, Login, and
Workspace**

Users of PATRIC can now register and create their own user-accounts. 
During registration, you can subscribe to the PATRIC Newsletter where
you’ll receive updates about data and software releases, upcoming
workshops, grant solicitations, presentations, and meetings. Once
registered, logging into your personal PATRIC account allows you to save
and manage the data groups you’ve gathered throughout the PATRIC site to
your personal Workspace. Future Workspace plans include allowing users
to save their preferences, thereby customizing searching and browsing at
PATRIC, and allowing users to upload their personal data in PATRIC and
incorporate it into our various visualization and analysis tools.

To read about the benefits of registration and register as a PATRIC
user, please visit:

https://patricbrc.org/portal/portal/patric/MyAccount

**New Integrated Text Mining**

Text mining capability, previously provided in PATRIC by the standalone
tool KLEIO, is now integrated as a component of the enhanced literature
search and text mining feature.  The text mining results are delivered
using technology developed in conjunction with the UK National Text
Mining Centre (`NaCTeM <http://www.nactem.ac.uk/>`__).  Text mining
results are based on indexes of UK Medline abstracts and identify key
entities from that text such as genes, proteins, metabolites, drugs,
diseases, symptoms, and other entities of interest. For a taxon, genome,
or gene of interest, results are available under the “Literature” tab.
Results are summarized by entity types and allow progressive filtering
of the results. Abstracts are also provided with key entities
highlighted in different colors.

For an example, select the Text Mining tab at:

http://patricbrc.org/portal/portal/patric/Literature?cType=taxon&cId=1386&time=a&kw=none

**PATRIC Now Has YouTube Tutorial and Use Case Videos**

Tutorials focus on general site navigation and features while Use Cases
offer more in-depth examples of gathering and analyzing data within
PATRIC.  Videos are available on `PATRIC’s YouTube
page. <http://www.youtube.com/user/PATRICBRC>`__

Videos can also be accessed from the About menu in the top navigation
bar of the PATRIC website or by visiting PATRIC eNews at
`http://enews.patricbrc.org/ <../../../../../>`__

**New Searches and Tools**
==========================

**Compare Region Viewer**

The new Compare Region Viewer, implemented using JBrowse and data APIs
provided by the SEED, allows researchers to compare genomic regions
around a gene of interest across other closely related genomes. Using
this viewer, one can quickly detect differences in translation start
sites, potential frame shifts, or missing genes. Coloring is based on
protein functions and allows users to visually group proteins with
similar functions. Users can also change the size of the region and
number of genomes compared.   This viewer can be accessed via the
Compare Region Viewer tab available on feature-level pages.

For an example see:

http://patricbrc.org/portal/portal/patric/CompareRegionViewer?cType=feature&cId=17814393&window=10000&regions=10

**Host-Pathogen Interactions**

PATRIC now offers a Host-Pathogen Interactions Search, which allows
users to find and visualize networks of experimentally-confirmed,
protein-protein interactions that occur between host and bacterial
proteins. Interaction data are collected from multiple public resources,
including BIND, DIP, GRID, IntAct, and MINT. Search tools allow users to
combine interaction networks from up to 12 bacteria, and also to filter
according to interaction type, detection method, and original source.
Results are displayed as an interactive graph and as a table of pairs of
interacting proteins. From either display, users can select subsets of
the data for download, alignment, and other actions; alternatively,
bacterial proteins can be saved to groups for later use.

The Host-Pathogen Interactions Search can be accessed from the Searches
and Tools menu in the top navigation bar of the PATRIC website or by
visiting:

http://patricbrc.org/portal/portal/patric/HPIFinder?cType=taxon&cId=&dm=

**ID Mapping Tool**

PATRIC’s new ID Mapping Tool is powered by UniProt’s ID Mapping service.
It allows users to quickly map PATRIC identifiers to those from other
prominent external databases such as GenBank, RefSeq, EMBL, UniProt,
KEGG, etc. Alternatively, users can start with list of external database
identifiers and map them to the corresponding features at PATRIC.

The ID Mapping tool can be accessed from the Searches and Tools menu in
the top navigation bar of the PATRIC website or by visiting:
http://patricbrc.org/portal/portal/patric/IDMapping?cType=taxon&cId=&dm\ =

This same ID Mapping tool is also available from the light blue Table
Toolbar on any of the search results or feature tables found throughout
the PATRIC site. Any feature(s) from tables or search results can be
selected.  Then clicking the “Map IDs” icon in the Table Toolbar and
selecting an external database will instantly convert these feature
identifiers to their corresponding identifiers in the database that was
selected.

For an example see:

http://patricbrc.org/portal/portal/patric/FeatureTable?cType=genome&cId=87468#key=178&pS=20&aP=1&dir=ASC&sort=genome_name,accession,start_max&sS=All&fT=CDS&alg=PATRIC&kW=

**Genomes and Annotations**
===========================

Between PATRIC’s Feburary 2011 release and April 2011, 132 new genomes
have been added and 23 genomes have been updated or replaced with the
newer versions. In total, 115 new genomes have been annotated using
RAST.

Twelve genomes previously present in PATRIC have since become obsolete
and were removed from the website. In addition, the Legacy BRC
annotations from 49 genomes have been removed from the database and
newer versions of these genomes have been updated with both RefSeq and
RAST annotations.

These Legacy BRC annotations are still available, but are now found
under the file download tab:
http://brcdownloads.vbi.vt.edu/patric2/LegacyBRC/

A Sequence Summary of the data currently available on the PATRIC website
through April, 2011 is provided in the table below:

.. raw:: html

   <table border="1" cellspacing="0" cellpadding="0">

.. raw:: html

   <tr>

.. raw:: html

   <td width="167">

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

Total Count

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

PATRIC Annotation

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

Legacy BRC Annotation

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

RefSeq Annotation

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="167">

Number of Genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

3252

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

2786

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

356

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

3192

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="167">

Number of Complete Genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

1369

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

1358

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

245

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

1353

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="167">

Number of WGS Genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

1486

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

1428

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

105

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

1443

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td width="167">

Number of Plasmid-only Genomes

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

397

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

6

.. raw:: html

   </td>

.. raw:: html

   <td width="69">

396

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </table>

View this Sequence Summary in addition to Genomic and Protein Feature
Summaries  on the PATRIC website:
http://patricbrc.org/portal/portal/patric/Taxon?cType=taxon&cId=2
