# Transcriptomics Gene List


## Transcriptomics Gene List Overview

A Gene List in PATRIC is a custom user-created list of genes based on
the transcriptomics datasets of interest. Each Gene List displays all of
the genes present in selected datasets, their functions, and summaries
of their expression levels in various samples or comparisons. A Gene
List can be dynamically filtered based on the identifiers/functions,
expression levels, or up/down regulation in one or more comparisons. Any
subset of genes of interest can be downloaded along with the annotations
and expression values as tab-delimited text or Excel file; or saved as a
Workspace group for further analysis. A complementary Heatmap Viewer
enables quick sorting or clustering of genes and comparisons; and
visualization of genes that are similarly expressed across one or more
comparison

## Accessing/Creating a Transcriptomics Gene List

A Gene List may be accessed while under the Transcriptomics Tab
(available on any Taxonomy or Genome level landing page) in the
following ways:

-   Select one or more Experiment(s) from either the Experiments Tab or
    the Comparisons Tab and then utilize the Table Toolbar, located in
    the light blue row to:
    -   Create a Gene List by clicking the Gene List button.
    -   Save selected items to groups within your Workspace by clicking
        the Add Feature(s) button. Your Workspace also contains a Table
        Toolbar with a Gene List button, where you may access the Gene
        List for the groups you create in your Workspace at any time.

-   From the Experiments Tab, click on links within the rows to navigate
    to the corresponding Gene List (Genes).
-   From the Comparisons Tab, click on links within the rows to navigate
    to the corresponding Gene List (Genes), list significant genes based
    on log ratio (|Log Ratio| &gt;= 1), or list significant genes based
    on Z-score (|Z-score| &gt;=2).

Note: To learn more about how to save data for future visits and utilize
your personal Workspace please see [Workspace FAQs](/content/Workspace_and_Groups). To learn about Transcriptomics and
Experiments and Comparisons Lists, see [Transcriptomics Experiment and
Comparison List FAQs](/content/Transcriptomics_Experiments_and_Comparisons).

## Filtering a Gene List

Both the Table and Heatmap Tabs can be filtered using the filet panel on
the left of the Gene List page in following ways:

-   Use the arrows to show genes that are up or down regulated in the
    subset of comparisons of interest.
-   Entering one or more keywords related to genome name, gene
    functions, or locus tags. Note: Separate multiple keywords/locus
    tags with a comma or a new line.
-   Based on the |Log Ratio| and/or |Z-score| cut-off of your choice.

## Gene List Table Table Features and Functionality

-   Sort the Gene List table as described in [Feature Table
    FAQs](/content/Feature_Table).
-   View the number of comparisons in which a gene is reported and
    up/down regulated. Click on the number to see the expression of the
    gene in those comparisons.
-   Use the Gene List Table Toolbar located in the light blue row to:
    -   Save selected items to groups within your Workspace by clicking
        the Add Feature(s) button. To learn more about how to save data
        for future visits and utilize your personal Workspace see
        [Workspace FAQs](/content/Workspace_and_Groups).
    -   View or download selected DNA and/or protein sequence data in
        FASTA format. The Gene List tables themselves, or selected data
        within them, are also downloadable in both excel and txt file
        formats.
    -   View pathways and associated pathway information for your
        selected genes by clicking the Pathway Summary button.
    -   Conduct Multiple Sequence Alignment analysis on selected groups,
        or selected items within groups, by clicking the Multiple
        Sequence Alignment button. For more details on this tool please
        see [Multiple Sequence Alignment
        FAQs](/content/Multiple_Sequence_Alignment).
    -   Utilize the ID Mapping Tool on selected items by clicking the
        Map IDs button. For more information on this tool please see [ID
        Mapping FAQs.](/content/ID_Mapping_Tool)
    -   Customize columns shown/hidden in your results table with the
        Columns button.


-   Click on any Locus Tag link within a row to visit the corresponding
    Gene landing page. From here you may:
    -   View information about the functional properties of the gene.
    -   Click on the Transcriptomics Tab to view expression of that gene
        across all available experimental datasets.
        -   Note: For more details on the transcriptomics data displayed
            at the gene level, please see [Gene Page Transcriptomics
            FAQs](/content/Gene_Page_Transcriptomics).
    -   Click on the Correlated Genes Tab to view other genes with
        correlated expression patterns.
    -   Utilize Tabs to see the gene in the Genome Browser, the Compare
        Region Viewer, associated Pathways, and Literature.
    -   Using buttons on the left, add the gene to your Workspace, or
        view the NT and/or AA sequences.

## How do I use the Gene List Heatmap Tab?

The Heatmap Tab visually displays expression levels of all the genes in
a Gene List across all selected comparisons using a Heatmap Viewer where
coloring is based on the Log Ratio value of a gene in a given
comparison. It allows you to quickly find genes with similar expression
patterns across one or more comparisons.

-   Use the Heatmap Toolbar located in the light blue row to:
    -   Flip Axes: By default, Comparisons are displayed along the X
        axis and Genes are displayed along the Y axis. Additionally, the
        scale of rows and columns may be controlled by sliding the x
        and/or y slidebars located at the axis intersection in the upper
        left corner of the Heatmap.
    -   Select Heatmap Color Scheme:
        -   Red-Black-Green: Up regulated genes are red and down
            regulated genes are green. The brighter the color, the more
            differentially expressed a gene is. All the genes that do
            not pass the current Log Ratio cut-off are black.
        -   Red-White-Blue: Up regulated genes are red and down
            regulated genes are blue. The brighter the color, the more
            differentially expressed a gene is. All the genes that do
            not pass the current Log Ratio cut-off are white.
    -   Press the Cluster button to reorder genes and comparisons in the
        Heatmap, allowing for quick visual detection of genes with
        similar expression patterns across one or more comparisons. This
        default mode of clustering uses Person correlation for distance
        measure and the pairwise complete-linkage method for
        hierarchical clustering.
    -   Press the Advance Clustering button to choose from various
        clustering algorithms and types.
    -   Show Significant Genes/All Genes: Choose to display either only
        Significant Genes passing Log Ratio and Z-score cut-offs or All
        Genes in the Heatmap. With All Genes selected and ordered based
        on genomic positions or locus tags, you may quickly find genomic
        regions that are differentially/similarly expressed across one
        or more comparisons.
-   The following options may be accessed from a pop-up widow by
    clicking on any individual colored cell, any Gene label, or any
    Comparison label within the Heatmap. The same information can be
    collected for a whole region of interest within the Heatmap by
    clicking and dragging to select a group of cells.
    -   Download expression data (Heatmap Data) for selected region.
    -   Download the list of genes as an Excel or txt file.
    -   Show Genes as an interactive Feature Table where the Table
        toolbar allows for sorting, downloading, and various analyses.
        For more details on how to use a Feature Table, see [Feature Table FAQs](/content/Feature_Table).
    -   Add Genes to a Group in your personal Workspace for future
        access.
