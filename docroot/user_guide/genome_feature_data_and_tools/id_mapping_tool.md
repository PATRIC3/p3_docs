# ID Mapping Tool

## Accessing the ID Mapping Tool on the PATRIC Website

This tool may be accessed from the MAP IDs Tools button in the light
blue Table Toolbar at the top of PATRIC tables, including the Table
Toolbar within your Workspace. It may also be accessed via the “Searches
and Tools” tab at the top of the PATRIC site. To learn more about PATRIC
Tables see [Feature Table FAQs](/content/Feature_Table).

## ID Mapping Overview

The ID Mapping Tool allows users to quickly map PATRIC identifiers to
those from other prominent external databases, such as GenBank, RefSeq,
EMBL, UniProt, KEGG, etc. Alternatively, users can start with a list of
external database identifiers and map them to the corresponding PATRIC
features.

## Using the ID Mapping Tool

-   To use the ID Mapping Tool from a Table Toolbar, simply select items
    in the table, click the
    ![16x16-toolbar-icon-idmapping](http://enews.patricbrc.org/wp-content/uploads/2013/04/16x16-toolbar-icon-idmapping.png){.alignnone
    .size-full .wp-image-2869 width="16" height="16"} MAP IDs Tools
    button, and chose an external database from the dropdown menu. Some
    example Use Cases include:
    -   Select a set of PATRIC features of interest from any PATRIC
        table and find corresponding identifiers in one of the external
        databases, such as RefSeq locus tags, GI numbers, UniProtKB
        Accessions etc.
    -   Select a set of PATRIC features of interest from any PATRIC
        table and find corresponding metabolic pathways at KEGG or
        BioCyc.
    -   Select a set of PATRIC features of interest from any PATRIC
        table and find corresponding protein structures in PDB.

-   To use the ID Mapping Tool from the “Searches and Tools” tab at the
    top of the PATRIC site, enter your identifiers in the box to the
    left and select “From” and “To” ID types from the dropdown menus on
    the right. Some example Use Cases include:
    -   Start with a set of external database identifiers, such as
        RefSeq locus tags, or UniprotKB Accessions, and find
        corresponding features in PATRIC.
        -   Note: You may enter your identifiers as either a list with
            one entry per line or multiple entries per line separated by
            commas.

## ID Mapping Sources

-   First, PATRIC CDSs (protein coding genes) are mapped to
    corresponding CDSs in RefSeq/GenBank by matching their stop position
    on genome sequences.
-   Second, RefSeq/GenBank CDSs are mapped to corresponding UniProtKB
    Accession.
-   Third, mappings are extended to other prominent external database
    identifiers using [UniProt’s ID Mapping
    Service](http://www.uniprot.org/mapping/).

PATRIC <-> RefSeq/GenBank <-> UniProtKB Accession <-> Other External Databases
