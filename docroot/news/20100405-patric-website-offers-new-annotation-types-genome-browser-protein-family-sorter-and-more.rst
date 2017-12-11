==========================================================================================
PATRIC Website Offers New Annotation Types, Genome Browser, Protein Family Sorter and More
==========================================================================================


:Date:   2010-04-05T16:34:40+00:00

Genomes and Annotations
=======================

-  The current PATRIC release includes RAST annotations for
   approximately 1,850 of the 2,000 complete bacterial genomes currently
   available in PATRIC.
   `RAST <http://www.patricbrc.org/portal/portal/patric/RAST>`__ (Rapid
   Annotation using Subsystem Technology, `Aziz et al.,
   2008 <http://www.ncbi.nlm.nih.gov/pubmed/18261238>`__) is a
   fully-automated service for annotating bacterial and archaeal
   genomes. It provides consistent and high quality genome annotations
   across the whole phylogenetic tree. Using a single annotation system
   across all bacterial genomes not only improves the consistency of
   annotations but also limits the noise and discrepancies that are
   difficult to rule out when multiple annotation systems are used.
-  This release also allows users to compare annotations from three
   different sources, including RAST, RefSeq, and legacy BRCs. When
   available, genomes have annotations from three different sources
   displayed side-by-side for easy comparison.
-  All genomes annotations are available through various pages on PATRIC
   website, including `Taxon
   Overview <http://www.patricbrc.org/portal/portal/patric/Taxon?cType=taxon&cId=262>`__,
   `Taxonomy <http://www.patricbrc.org/portal/portal/patric/TaxonomyTree?cType=taxon&cId=262>`__,
   `Genome
   List <http://www.patricbrc.org/portal/portal/patric/GenomeList?cType=taxon&cId=262>`__,
   `Feature
   Table <http://www.patricbrc.org/portal/portal/patric/FeatureTable?cType=taxon&cId=262>`__,
   `Genome
   Overview <http://www.patricbrc.org/portal/portal/patric/Genome?cType=genome&cId=90181>`__.
   All of these pages are available as tabs, seen directly under the
   Taxonomy Overview.

.. raw:: html

   <table border="1" cellspacing="0" width="100%">

.. raw:: html

   <tr>

.. raw:: html

   <th>

.. raw:: html

   </th>

.. raw:: html

   <th align="left">

PATRIC

.. raw:: html

   </th>

.. raw:: html

   <th align="left">

Legacy BRC

.. raw:: html

   </th>

.. raw:: html

   <th align="left">

RefSeq

.. raw:: html

   </th>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Number of genomes

.. raw:: html

   </td>

.. raw:: html

   <td class="right">

2,135

.. raw:: html

   </td>

.. raw:: html

   <td class="right">

410

.. raw:: html

   </td>

.. raw:: html

   <td class="right">

2,577

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Number of genomic features

.. raw:: html

   </td>

.. raw:: html

   <td class="right">

15,495,850

.. raw:: html

   </td>

.. raw:: html

   <td class="right">

2,324,786

.. raw:: html

   </td>

.. raw:: html

   <td class="right">

16,647,467

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </table>

Website Enhancements
====================

Genome Browser
--------------

-  PATRIC now offers Ajax-based genome browser implemented using JBrowse
   (`Skinner et al,
   2009 <http://www.ncbi.nlm.nih.gov/pubmed/19570905>`__). Access to the
   browser, via tabs, is available at both the `genome and feature
   levels <http://www.patricbrc.org/portal/portal/patric/GenomeBrowser?cType=genome&cId=90181&loc=NC_007880:0..10000&tracks=DNA,CDS%28PATRIC%29,gene%28PATRIC%29,RNA%28PATRIC%29>`__.
   Links to the genome browser are also available from the `Genome
   List <http://www.patricbrc.org/portal/portal/patric/GenomeList?cType=taxon&cId=262&dataSource=PATRIC&displayMode=genome>`__
   and the `Feature
   Table <http://www.patricbrc.org/portal/portal/patric/FeatureTable?cType=genome&cId=90181>`__.

   -  The new browser has tracks for genes, CDSs, RNAs and other
      miscellaneous features. The browser also allows users to compare
      the three annotation systems (RefSeq, PATRIC/RAST and Legacy BRC)
      simultaneously. Each is available by a separate track, allowing
      the user to do a comparative analysis.

Protein Family Sorter
---------------------

-  The current PATRIC release provides functional protein families. The
   families are created using FIGfams, generated from RAST annotations,
   and allow the user to look at protein conservation among diverse
   bacterial orders.

   -  `Protein Family
      Sorter <http://www.patricbrc.org/portal/portal/patric/FIGfamSorter?cType=taxon&cId=>`__
      allows the users to include or exclude genomes, and also to put
      genomes into a “don’t care” category, offering more diversity in
      sorting ability. Users can also filter by family description or
      FIGfam number.
   -  Information on all families, or on individual members of a
      specific family, is available by download to either excel or text.
   -  Multiple sequence alignments are generated when requested. They
      open in a new window.

Metabolic Pathways
------------------

-  PATRIC now offers metabolic pathways using
   `KEGG <http://www.genome.jp/kegg/>`__ pathway maps. EC numbers that
   are annotated by RefSeq, PATRIC/RAST or the legacy BRCs are mapped to
   KEGG pathways. The user can see which annotation system has
   identified a specific EC on any pathway map allowing a comparative
   approach.

   -  Pathways are available at both `genome and feature
      levels <http://www.patricbrc.org/portal/portal/patric/PathwayTable?cType=genome&cId=90181&viewtype=PATH>`__.

Phylogenetic Trees
------------------

-  In this release PATRIC provides Order-level `phylogenetic
   trees <http://www.patricbrc.org/portal/portal/patric/Phylogeny?cType=taxon&cId=262>`__
   for all pathogenic bacteria. These trees show members of the order,
   and also show details of the parts of the tree that contain the
   pathogenic genera, which are highlighted in red.

Searches and Tools
------------------

-  A new `Pathway
   Search <http://www.patricbrc.org/portal/portal/patric/PathwayFinder?cType=taxon&cId=>`__
   allows user to search pathway data using EC numbers, pathway IDs, or
   pathway names. Search can be narrowed to a group of genomes using the
   taxonomy tree, or can be open to all bacteria. Users can also filter
   by annotation source (RefSeq, PATRIC/RAST, legacy BRCs, or all).

   -  An improved `BLAST
      Search <http://www.patricbrc.org/portal/portal/patric/Blast>`__
      now provides analysis by all flavors (blastn, blastp, blastx,
      tblastn, tblastx) against the genes and protein sequences from
      RefSeq, PATRIC/RAST and the legacy BRC annotations. BLAST can also
      be performed against genome sequences.
