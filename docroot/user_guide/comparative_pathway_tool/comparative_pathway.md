# Comparative Pathway Tool

## Accessing the Comparative Pathway Tool on the PATRIC Website

An advanced search, described below, may be conducted from the “Searches
and Tools” tab at the top of the PATRIC site and from the “Search Tools”
box on any Organism Landing page. To learn about Organism Landing pages,
see the [PATRIC Data Organization Overview
tutorial](http://enews.patricbrc.org/patric-data-organization-overview/).

-   Note: Searches conducted using Comparative Pathway Tool from the
    “Search Tools” box on an Organism Landing page will be pre-scoped to
    the taxonomic level of the page.

## Comparative Pathway Tool Overview

The Comparative Pathway Tool allows you to identify a set of pathways
based on taxonomy, EC number, pathway ID, pathway name and/or specific
annotation type. The Comparative Pathway Tool displays a table of unique
pathways that match the search criteria. From there, you can select
specific pathways of interest and view the Comparative Pathway KEGG Map
and the Comparative Pathway Heatmap.

## Using the Comparative Pathway Tool

To begin, conduct an initial search by 1) selecting your phylum, class,
order, family, genus, species, or genomes of interest via the Taxonomy
Tree tab, the Alphabetized Organism tab, or begin typing in the “Jump
to” field 2) utilizing the Keyword search functionality, or 3) a
combination of both. Then click on the Search button. Note: Larger
searches may take PATRIC several minutes. For an explanation of various
annotation sources, please see [Annotation
FAQs.](/content/Genome_Annotations)

Results will be shown in a Pathway table. From here you may do the
following:

-   Use the three tabs (Pathways, EC number, and Genes) at the top of
    the table to navigate your search results. Click on links within
    rows under each tab to navigate to the various pages:
    -   From the Pathway tab you can navigate within rows to a specific
        PATRIC Pathway Map page (Pathway Name), a table with all the EC
        numbers annotated in a particular pathway (Unique EC Count), and
        a table with all the genes in a particular pathway (Unique Gene
        Count).
    -   From the EC Number tab you can navigate within rows to a
        specific PATRIC Pathway Map page (Pathway Name), a table with
        all the genes for a particular EC number (Unique Gene Count).
    -   From the Genes tab you can navigate within rows to specific
        PATRIC genome pages (Genome Name), NCBI nucleotide pages for
        that genome (Accession), specific PATRIC locus pages (Locus
        Tag), or a specific PATRIC Pathway Map page (Pathway Name).
        -   Note: The Accession column is not shown in the default view.


-   Use the column headers to sort your search results.

-   Use the Pathway Table Toolbar, located in the light blue row at the
    top of the table to:
    -   Save selected items to groups within your Workspace by clicking
        the Add Feature(s) button. To learn more about how to save data
        for future visits and utilize your personal Workspace please see
        [Workspace FAQs](/content/Workspace_and_Groups).
    -   View or download selected DNA and/or protein sequence data in
        FASTA format. The table itself, or selected data within it, are
        also downloadable in both excel and txt file formats.
    -   View pathways and associated pathway information for your
        selected genes by clicking the Pathway Summary button.
    -   Conduct Multiple Sequence Alignment analysis on selected
        features by clicking the Multiple Sequence Alignment button. For
        more details on this tool please see [Multiple Sequence
        Alignment FAQs](/content/Multiple_Sequence_Alignment).
    -   Utilize the ID Mapping Tool on selected features by clicking the
        Map IDs button. For more information on this tool please see [ID
        Mapping FAQs.](/content/ID_Mapping_Tool)
    -   Customize columns shown/hidden in your results table with the
        Columns button.

-   Click on any Pathway Name to view results via the default KEGG Map
    tab or the Heatmap Tab. For details on how to use these tools,
    please see [Comparative KEGG Map
    FAQs](/content/Comparative_Pathway_KEGG_Map) and [Comparative
    Pathway Heatmap FAQs.](/content/Comparative_Pathway_Heatmap)

## Comparative Pathway Tool Information

-   **Genome Count**: This gives the number of genomes that have some
    genes present in this pathway at the taxonomic level chosen.

-   **Unique Gene Count**: This provides a list of all the genes in all
    the genomes that belong to this pathway. Clicking on any number in
    this column will provide a list of the annotated genes in each
    genome that belong to this family.

-   **Unique EC Count**: The Enzyme Commission number (EC number) is a
    numerical classification scheme for enzymes, based on the chemical
    reactions they catalyze and in a given KEGG metabolic pathway, each
    step has an EC number assigned to it. In a given genome there may be
    several genes that have been assigned the same EC number, meaning
    that several different genes have the possibility of doing the same
    job. The unique EC count tells how many steps within the pathway
    have at least one gene behind them.

-   **EC Conservation %**: For a single pathway (row), this number gives
    the percent of unique EC numbers present in all selected genomes.
    100% describes a situation in which all unique EC numbers are
    present in all selected genomes. Smaller numbers indicate that there
    is one or more genomes are missing some EC numbers.

-   **Gene Conservation**: A genome can have several genes that have
    been assigned the same EC number. Gene conservation provides an
    estimate of pathways where there might be redundancies, or where EC
    numbers are missing. Numbers greater than one mean that in at least
    one genome, there is more than one gene that has been assigned a
    particular EC number. Numbers less than one mean indicate that in at
    least one genome, a particular EC number is missing. This provides a
    quick way to see which pathways have perfect conservation across all
    genomes (Gene Conservation = 1) to those pathways where there are
    differences among the genomes. Users can then explore these
    differences by drilling down on either the Unique Gene Count, or the
    Unique EC Count.
