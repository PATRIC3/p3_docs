Protein Family Heatmap
======================

Accessing the Protein Family Heatmap on the PATRIC Website
----------------------------------------------------------

This tool is accessible via the “Heatmap” Tab on the initial search
results page generated within our Protein Family Sorter Tool. For
information on how to use the Protein Family Sorter please see `Protein
Family Sorter FAQs </content/Protein_Family_Sorter>`__.

Protein Family Heatmap Overview
-------------------------------

The Heatmap is an interactive visualization tool, which provides an
overview of the distribution of proteins across a selected set of
genomes. Patterns visible in a Heatmap can allow for many types of
analysis such as, a bird’s-eye view of the conservation (or lack
thereof) of particular genes of interest, discerning how many proteins
have the same function within a single genome, and identifying proteins
with multiple homologs or paralogs across a set of genomes.

Color Coding
------------

Each cell is colored according to how many proteins from a specific
genome are members of a given protein family. Black cells indicate that
there are no representative proteins from a specific genome for that
protein family. Bright yellow cells indicate there is one representative
protein, dark yellow cells indicate there are two representative
proteins, and dark orange cells indicate there are three or more
representative proteins.

Table Filter Panel
------------------

Both the Table and Heatmap tabs may be filtered using this panel. The
Genome Filter at the top of the panel allows for the following three
filter selections to be made for each genome:

-  Selecting "resent in all Families" will show only protein families
   that include members from those selected genomes.
-  Selecting "Absent from all Families" will show only protein families
   that do not include members from those selected genomes.
-  Selecting “Either/Mixed” specifies that proteins from selected
   genomes may or may not be included in the resulting protein family
   list. This option is set by default, and allows users to focus on
   only those genomes they want to include and/or exclude without having
   to explicitly set one of these two options for every genome.

Five Genome Metadata categories are also available to filter on (i.e.
search for protein families that are present in genomes isolated from
host A but absent in genomes from host B). The categories include
country of isolation, host, disease, collection date, and completion
date and are accessible by grabbing the right edge of the Filtering
Panel and expanding it out.

The Filters at the bottom of the panel enable narrowing of the results
based on Keywords, Perfect Families, and/or the number of proteins or
genomes per protein family.

Note: PATRIC can not filter searches yielding more than 400 genomes.

Data Sorting
------------

-  The entire visualization may be sorted by choosing a reference genome
   to act as an anchor. This will automatically sort all the protein
   families based on the gene order in that genome. To select a
   reference genome, either chose one from the “Sort Protein Families
   by” field at the top of the Heatmap or click on any genome in the
   Heatmap and then click the “Sort Protein Families” button in the
   pop-up window.

This functionality allows the user to quickly identify groups of
contiguous genes present or absent in one or more of the selected
genomes. In addition, the user can quickly visualize areas of loss or
gain of genomic segments across genomes that are closely or more
distantly related. Some of these areas may correspond to pathogenicity
islands.

-  Each individual column or row within the Heatmap may also be clicked
   and dragged to any specified position.

Protein Family Heatmap Features and Functionality
-------------------------------------------------

-  Genomes are listed along the Y (vertical) axis and corresponding
   protein families are listed along the X (horizontal) axis. The scale
   of these rows and columns may be controlled by sliding the x and/or y
   slidebars located at the axis intersection in the upper left corner
   of the Heatmap.
-  Click on the Cluster button to show hierarchical clustering that
   allows for quick visual detection of genes with similar expression
   patterns across one or more comparisons.

   -  Note: The default settings for the clustering button are based on
      the Pearson Correlation Algorithm and a Pairwise Average-linkage
      Clustering Type. If you click on the Advanced Clustering button,
      you may choose from several different distance measures and
      clustering methods to be performed.

-  Use the Flip Axis button to arrange the Heatmap to better visualize
   your particular data set of interest.

-  The following options may be accessed from a pop-up widow by clicking
   on any individual colored cell within the Heatmap, any Genome label,
   or any Protein Family label. The same information can be collected
   for a whole region of interest within the Heatmap by clicking and
   dragging to select a group of cells.

   -  The “Download Heatmap Data” button will show the count of
      representative proteins for each genome in either a text or excel
      file. Note: Clicking this button from a Genome label will produce
      a file with the count for each protein family within that genome,
      while clicking on this button from a Protein Family label will
      produce a file with the count for that particular protein family
      in every genome where it is found.
   -  The “Add Proteins to Group” button will save selected items to
      new, or existing, groups within your Workspace. To learn more
      about how to save data for future visits and utilize your personal
      Workspace please see `Workspace
      FAQs </content/Workspace_and_Groups>`__.
   -  Data for each protein, such as Genome Name, Locus Tag, Start and
      End designations, Overall Length, and Product Description may be
      obtained in several ways:

      -  Clicking the “Download Proteins” button will open the protein
         data in either a text or excel file.
      -  Clicking the “Show Proteins” button will open the protein data
         within a Protein Families Table, where the Toolbar, located in
         the light blue row of the table may be utilized to:

         -  Save selected items to groups within your Workspace by
            clicking the Add Feature(s) button. To learn more about how
            to save data for future visits and utilize your personal
            Workspace please see `Workspace
            FAQs </content/Workspace_and_Groups>`__.
         -  View or download selected DNA and/or protein sequence data
            in FASTA format. The table itself, or selected data within
            it, are also downloadable in both excel and txt file
            formats.
         -  View pathways and associated pathway information for your
            selected genes by clicking the Pathway Summary button.
         -  Conduct Multiple Sequence Alignment analysis on selected
            features by clicking the Multiple Sequence Alignment button.
            For more details on this tool please see `Multiple Sequence
            Alignment FAQs </content/Multiple_Sequence_Alignment>`__.
         -  Utilize the ID Mapping Tool on selected features by clicking
            the Map IDs button. For more information on this tool please
            see `ID Mapping FAQs. </content/ID_Mapping_Tool>`__
         -  Customize columns shown/hidden in your results table with
            the Columns button.

Note: All tables accessed via the Protein Family Heatmap may be sorted
as described in `Feature Table FAQs </content/Feature_Table>`__.
