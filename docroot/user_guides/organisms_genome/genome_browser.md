# Genome Browser

## Accessing the Genome Browser on the PATRIC Website

Each Organism on PATRIC has an Organism Landing Page. To get to this
page at the Genus level, select your Genera of interest from the
Organisms tab on the PATRIC homepage. The phylogeny of each Landing Page
is listed across the top of the page. Once on the Genera Landing Page,
you may access the Genome Browser by drilling down in one of the
following ways to either the Genome or the Feature level:

-   Select the Genome List tab and click on your Genome Name of
    interest. This will take you to the chosen Genome-level Landing
    Page. At all Genome and Feature-level Landing Pages, the Genome List
    tab at the top of the page changes to a Genome Browser tab providing
    direct access to the Tool.
-   Select the Genome List tab and click on any Genome Browser icon
    within the table to visually explore a specific genome.

-   Select the Feature Table tab and click on any Genome Browser icon
    within the table.

You may also access the Genome Browser from within any PATRIC table you
create while using PATRIC Searches and Tools where you see the Genome
Browser icon.

## Genome Browser Overview

The Genome Browser is a graphical representation of the alignment of
genes and other genomic data depicted along a central horizontal axis of
genome coordinates.

### Genome Browser Features and Functionality

Genome Browser Main Window:

-   Pan to a region of interest in the genome by:
    -   Using the forward and backward arrow buttons at the top of the
        Browser.
    -   Clicking and dragging the red slide bar located within the
        genome coordinate axis.
    -   Entering your own start and/or end coordinates in the coordinate
        field and clicking on the “Go” button.

-   Zoom in/out to regions of interest by using the + and – buttons
    along the top of the Browser. The larger buttons will zoom further
    in/out with one click than the smaller buttons.

Note: Once you reach a zoom level of approximately 1,300 base pairs or
less a color-coded DNA sequence track (with associated AAs) will appear
for the Reference Sequence. Zooming in to 150 base pairs or less will
label the NAs and AAs with the corresponding letter.

A = green, T = red , C = blue , G = yellow.

-   Any specific area you are viewing in the genome browser may be saved
    for the future via clicking the “Link” button in the upper right.
    Copy this url and share it or save it and visit the same area at
    another time.
-   Using a yellow highlighter, you may highlight a region of the
    browser. To do this either select the highlighter icon (in the zoom
    bar) and then click and drag an area of the browser window or use
    the View menu in the top left. Clear highlighted sections via the
    View menu.

Note: A highlighted notation will remain when using the Link tool.

Interacting with Browser Tracks and Downloading Track/Sequence Data:

-   The Genome Browser will initially open showing both PATRIC (blue)
    and RefSeq (green) annotated data tracks.
-   Additional tracks, such as those annotated by Legacy BRCs, are
    located in the Available Tracks column, along the left side of the
    Genome Browser.
    -   To add or remove tracks from the Genome Browser, simply click
        and drag them between the “Available Tracks” column and the
        browser window.
    -   You may also remove tracks from the browser window by clicking
        on “Remove Track” from the drop-down menu next to the annotation
        source label or clicking on the “x” on the annotation source
        label.
-   From the drop down menu (accessed by hovering over the Reference
    sequence track label,) you may see information about the track, pin
    the track to the top row in the browser, edit the tracks
    configuration, remove the track to the Available Tracks column, save
    track data, and chose to show/hide forward strand, reverse strand,
    and translation.
    -   When saving track data, you may chose to view or download either
        the “visible region” or the “whole reference genome” in FASTA
        format.
-   From the drop down menu (accessed by hovering over any Annotation
    track label,) you may see information about the track, pin the track
    to the top of the row in the browser, edit the tracks configuration,
    remove the track to the Available Tracks column, save the track
    data, or show/hide feature labels.
    -   When saving track data, you may chose to view or download either
        the “visible region” or the “whole reference genome” in one of
        the three following formats: GFF3, BED, or Sequin Table.

Uploading Your Own Tracks and Adding Custom Tracks:

-   Upload and view your own annotations or gene lists as GFF3 files and
    view them as tracks on the genome browser by selecting “Open” from
    the File menu in the top left corner of the browser.
-   Upload and view your RNA-Seq, ChIP-Seq, or SNP data as BigWig or BAM
    files and view them as tracks in the genome browser by selecting
    “Open” from the File menu in the top left corner of the browser.
-   You may also create tracks showing specific regions of the Reference
    Sequence (or it’s translations) by entering the NA or AA sequence.
    To do this, select “Add sequence search track” from the file menu.

Interacting with Individual Browser Features and Accessing Feature
Sequence Data:

-   Different genomic feature types annotated by the same source are
    grouped together as single tracks, using various shades of the same
    color to represent different feature types. i.e. PATRIC annotations,
    shown in blue, will range from light blue to darker blue depending
    on the feature type.
-   Hovering over any feature within the Browser will display
    information such as Locus Tag, Location, Strand, Type, Gene Symbol,
    and Product.
-   Clicking on any feature within the Browser will open a pop-up with
    feature details and, if applicable, links to the Genome Browser,
    Compare Region Viewer, Associated Pathways, Transcriptomics Data,
    and Correlated Genes for that particular feature. The pop-up also
    contains the NA sequence for the feature.

### Source

PATRIC offers Ajax-based genome browser implemented using JBrowse
([Skinner et al, 2009](http://www.ncbi.nlm.nih.gov/pubmed/19570905)).
