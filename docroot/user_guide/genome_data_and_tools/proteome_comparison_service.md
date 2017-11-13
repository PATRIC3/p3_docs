# Proteome Comparison Service

## Overview
The Proteome Comparison Service performs protein sequence-based genome comparison using bidirectional BLASTP. This service allows users to select up to eight genomes, either public or private, and compare them to a user-selected or supplied reference genome. The genome comparison result is displayed as an interactive circular genome view and are downloadable as a print-quality image or tabular comparison results.

The Proteome Comparison Service can be accessed from the Services Menu at the top of the PATRIC website page.

## Parameters

### Advanced parameters:

#### Minimum % coverage
Minimum percent sequence coverage of query and subject in blast.
Use up or down arrows to change the value. The default value is 30%.

#### Blast e-value
Maximum blast e-value. A default value of 1e-5 is used if leave blank.

#### Minimum % identity
Minimum percent sequence identity of query and subject in blast. Use up or down arrows
to change the value. The default value is 10%.

### Output Folder
The workspace folder where results will be placed.

### Output Name
Name used to uniquely identify results.

## Reference Genome Selection
Select a reference genome from the genome list or a fasta file or a
feature group. Only one reference is allowed.

### Select a genome
Type or select a genome name from the genome list.

### Or a fasta file
Select or upload an external genome file in protein fasta format.

### Or a feature group
Select a feature group from the workspace to show comparison of specific proteins instead of all proteins in a genome.

## Comparison Genomes Selection
Select up to total of 9 genomes from the genome list or fasta files or a
feature groups and use the plus buttons to place the genomes to the
table .

### Select genome
Type or select a genome name from the genome list.

### And/or select fasta file
Select or upload an external genome file in protein fasta format.

### And/or select feature group
Select a feature group from the workspace.
