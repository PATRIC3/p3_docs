# Metagenome Binning Service

## Overview
The Metagenomic Binning Service accepts either reads or contigs, and attempts to "bin" the data into a set of genomes. This service can be used to reconstruct bacterial and archael genomes from environmental samples. This webinar provides an example analysis that demonstrates how to use the service and interpret the results.

### See also
* [Metagenome Binning Service](https://patricbrc.org/app/MetagenomeBinning)
* [Metagenome Binning Service Tutorial](https://docs.patricbrc.org//tutorial/metagenomic_binning/metagenomic_binning.html)

## Using the Metagenome Binning Service
The **Metagenome Binning** submenu option under the **Services** main menu (Genomics category) opens the Metagenome Binning Service input form (*shown below*). *Note: You must be logged into PATRIC to use this service.*

![Metagenome Binning Menu](../images/services_menu.png)

## Options
![Metagenome Binning Input Form](../images/metagenome_binning_input_form.png) 

## Paired read library

### Read File 1 & 2
Many paired read libraries are given as file pairs, with each file containing half of each read pair. Paired read files are expected to be sorted such that each read in a pair occurs in the same Nth position as its mate in their respective files. These files are specified as READ FILE 1 and READ FILE 2. For a given file pair, the selection of which file is READ 1 and which is READ 2 does not matter.

### Advanced Parameters

#### File 1 Interleaved
Some paired libraries are available in a single file where each read in a pair occurs in succession. To specify such a file set this parameter to 'True'.

#### Mean Insert Size
This refers to the mean insert size between paired reads. If you have this information you may provide it. If not the assembly algorithm will make an attempt to determine this value.

#### Std. Insert Size
This refers to the standard deviation of the insert size between paired reads. If you have this information you may provide it. If not the assembly algorithm will make an attempt to determine this value.

#### Mate Paired
Defines the orientation of read pairs. Setting Mate Paired to true indicates that the sequencing direction of the two reads in each pair is outward facing.

#### Platform
The sequencing platform used for each library.
  - infer: Infer sequencing platform from read files
  - illumina: Illumina short reads
  - pacbio: PacBio long reads
  - nanopore: MinION long reads

## Parameters

### Output Folder
The workspace folder where results will be placed.

### Output Name
Name used to uniquely identify results.

### Genome Group Name
Name used to create genome group with identified genomes.
