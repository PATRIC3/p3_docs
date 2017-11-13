# RNA-Seq Analysis

## Overview
The RNA-Seq Analysis Service provides services for aligning, assembling, and testing differential expression on RNA-Seq data. The service provides three recipes for processing RNA-Seq data: 1) Rockhopper, based on the popular Rockhopper tool for processing prokaryotic RNA-Seq data; 2) Tuxedo, based on the tuxedo suite of tools (i.e., Bowtie, Cufflinks, Cuffdiff); and 3) and HISAT2 for host (human, etc.) reference genomes. The service provides SAM/BAM output for alignment, tab delimited files profiling expression levels, and differential expression test results between conditions. A tutorial for using the RNA-Seq Analysis Service is available here.

The RNA-Seq Service can be accessed from the Services Menu at the top of the PATRIC website page and via the PATRIC Command Line Interface (CLI).

## Parameters

### Strategy
This parameter governs the software used to align, assemble, quantify,
and compare reads from different samples.

#### Rockhopper
Runs the [Rockhopper
software](http://nar.oxfordjournals.org/content/41/14/e140) designed for
RNA-Seq on prokarytoic organisms. With this strategy selected Rockhopper
will handle all steps (alignment, assembly, quanitification, and
differential expression testing).

#### Tuxedo
Runs the [tuxedo
strategy](http://www.nature.com/nprot/journal/v7/n3/abs/nprot.2012.016.html)
using Bowtie2, Cufflinks, and CuffDiff to align, assemble, and compare
samples respectively. This is a similar strategy as used by
[RNA-Rocket](http://bioinformatics.oxfordjournals.org/content/31/9/1496).

#### Host HISAT2
Runs HISAT2 for alignment against the selected host and then uses the
remainder of the Tuxedo strategy. [tuxedo
strategy](http://www.nature.com/nprot/journal/v7/n3/abs/nprot.2012.016.html)
using Cufflinks, and CuffDiff to assemble, and compare samples
respectively.

### Output Folder
The workspace folder where results will be placed.

### Output Name
Name used to uniquely identify results.

## Paired read library

### Read File 1 & 2
Many paired read libraries are given as file pairs,
with each file containing half of each read pair. Paired read files are
expected to be sorted such that each read in a pair occurs in the same
Nth position as its mate in their respective files. These files are
specified as READ FILE 1 and READ FILE 2. For a given file pair, the
selection of which file is READ 1 and which is READ 2 does not matter.

### Condition
The group/condition specified will be used to determine contrasts in the
differential expression portion of the analysis. Each group will be
compared to every other group in all vs. all fashion. Reads assigned to
the same group will be used as replicates.

## Groups/Conditions
Turning on Groups/Conditions also turns on differential expression
analysis. In this panel the user has the ability to specify conditions
that can be assigned to read libraries. When this option is enabled each
read library moved to the "Selected libraries" panel must have a group
designation. Read libraries assigned to different groups will be
compared for differential expression in all vs. all fashion. Two or more
read libraries marked with the same group will be regarded as
replicates.

## Selected libraries
Read files placed here will contribute to a single RNA-Seq analysis. If
the Groups/Conditions option is turned on, read files placed into this
table under the same group will be considered replicates.
