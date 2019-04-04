# Metagenomic Read Mapping Service

## Overview
The Metagenomic Read Mapping Service uses KMA to align reads against antibiotic resistance genes from CARD and virulence factors from VFDB.

### See also
  * [Metagenomic Read Mapping Service](https://patricbrc.org/app/MetagenomicReadMapping)

## Using the Metagenomic Read Mapping Service
The **Metagenomic Read Mapping** submenu option under the **Services** main menu (Metagenomics category) opens the Metagenomic Read Mapping Service input form (shown below). *Note: You must be logged into PATRIC to use this service.*

![Metagenomic Read Mapping Service Menu](../images/services_menu.png)

## Options
![Metagenomic Read Mapping Service Input Form](../images/metagenomic_read_mapping_input_form.png)

## Input File

### Paired read library

**Read File 1 & 2:**  Many paired read libraries are given as file pairs, with each file containing half of each read pair. Paired read files are expected to be sorted such that each read in a pair occurs in the same Nth position as its mate in their respective files. These files are specified as READ FILE 1 and READ FILE 2. For a given file pair, the selection of which file is READ 1 and which is READ 2 does not matter.

### Single read library

**Read File:**
The fastq file containing the reads

### SRA run accession
Allows direct upload of read files from the [NCBI Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) to the PATRIC Assembly Service. Entering the SRR accession number and clicking the arrow will add the file to the selected libraries box for use in the assembly. 

### Selected libraries
Read files to be mapped.

## Parameters

**Gene Set Type:** The set of genes against which to map.  Three options are available:

* 


**Predefined Gene Set Name:**


**Save Classified Reads:** 


**Save Unclassified Reads:** 

**Output Folder:** Workspace folder where the results will be saved.

**Output Name:** User-provided name used to uniquely identify results.


## Output Results
![Metagenomic Read Mapping Service Output Files](../images/metagenomic_read_mapping_output_files.png)

The Metagenomic Read Mapping Service generates several files that are deposited in the Private Workspace in the designated Output Folder. These include

 
