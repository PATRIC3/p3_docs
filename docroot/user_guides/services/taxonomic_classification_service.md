# Taxonomic Classification Service

## Overview
The Taxonomic Classification Service accepts reads or contigs from sequencing of a metagenomic sample and uses [Kraken 2](http://genomebiology.com/2014/15/3/R46) to assign the reads to taxonomic bins, providing an initial profile of the possible constituent organisms present in the sample.

### See also
  * [Taxonomic Classification Service](https://patricbrc.org/app/TaxonomicClassification)
  * Taxonomic Classification Service Tutorial - TBD
  * [Metagenome Binning Service](./metagenome_binning_service.html)

## Using the Taxonomic Classification Service
The **Taxonomic Classification** submenu option under the **Services** main menu (Metagenomics category) opens the Taxonomic Classification input form (shown below). *Note: You must be logged into PATRIC to use this service.*

![Taxonomic Classification Menu](../images/services_menu.png)

## Options
![Taxonomic Classification Input Form](../images/taxonomic_classification_input_form_v2.png)

## Start With
The service can accept either read files or assembled contigs. If the "Read File" option is selected, the form will provide controls to allow input of read files or SRA accession numbers.  If the "Assembled Contigs" option is selected, the form will change to allow input of a contig file.   

## Input File
Depending on the option chosen above (Read File or Assembled Contigs), the Input File section will request read files or assembled contigs, respectively.

### Paired read library
**Read File 1 & 2:**  Many paired read libraries are given as file pairs, with each file containing half of each read pair. Paired read files are expected to be sorted such that each read in a pair occurs in the same Nth position as its mate in their respective files. These files are specified as READ FILE 1 and READ FILE 2. For a given file pair, the selection of which file is READ 1 and which is READ 2 does not matter.

### Single read library
**Read File:** The fastq file containing the reads.

### SRA run accession
Allows direct upload of read files from the [NCBI Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) to the PATRIC Assembly Service. Entering the SRR accession number and clicking the arrow will add the file to the selected libraries box for use in the assembly.

## Selected libraries
Read files placed here will contribute to a single assembly.

## Parameters

### Algorithm

 * [Kraken 2](http://genomebiology.com/2014/15/3/R46) - Assigns taxonomic labels to metagenomic DNA sequences using exact alignmnet of k-mers.

### Database
Reference taxonomic database used by the algorithm.

* [All genomes](https://ccb.jhu.edu/software/kraken2/index.shtml?t=manual#standard-kraken-2-database) - Standard Kraken 2 database containing distinct 31-mers, based on completed microbial genomes from NCBI.
* [RDP (SSU rRNA)](https://academic.oup.com/nar/article/25/1/109/1083216) - The Ribosomal Database Project (RDP), a naïve Bayesian-based classification for bacterial 16S rRNA sequences.
* [SILVA (SSU rRNA)](https://doi.org/10.1093/nar/gkt1209) - Comprehensive database of aligned ribosomal RNA (rRNA) gene sequences from the Bacteria, Archaea and Eukaryota domains and supplementary online services. 

### Output Folder
The workspace folder where results will be placed.

### Output Name
Name used to uniquely identify results.

## Output Results
![Taxonomic Classification Output Files](../images/taxonomic_classification_output_files_v2.png)

The Taxonomic Classification Service generates several files that are deposited in the Private Workspace in the designated Output Folder. To reivThese include

 * **TaxonomicReport.html** - A web-browser-viewable report that summarizes the results of the service including
   * Input Data - read files used
   * Results - a table of the top taxonomic hits
   * Link to interactive chart showing the taxonomic classification distribution
 * **chart.html** - Link to [Krona](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3190407/)-based interactive chart showing the taxonomic classification distribution (see image below)
 * **classified_1.fastq.gz** - reads that were classified by Kraken 2 *(only if Save Classified Sequences option is chosen)*
 * **classified_2.fastq.gz** - reads that were classified by Kraken 2 *(only if Save Classified Sequences option is chosen)*
 * **full_report.txt** - Full Kraken 2 report; includes zero counts (see [Kraken 2 Output Formats](https://ccb.jhu.edu/software/kraken2/index.shtml?t=manual#output-formats))
 * **output.txt.gz** - Per-read Kraken 2 output file
 * **report.txt** - Kraken 2 report; suppresses zero counts
 * **unclassified_1.fastq.gz** - reads that were not classified by Kraken 2 *(only if Save Unclassified Sequences option is chosen)*
 * **unclassified_2.fastq.gz** - reads that were not classified by Kraken 2 *(only if Save Unclassified Sequences option is chosen)*

![Krona-based interactive Taxonomic Classification Chart](../images/krona_taxonomic_classification_chart.png)

### Action buttons
After selecting one of the output files by clicking it, a set of options becomes available in the vertical green Action Bar on the right side of the table.  These include

* **Hide/Show:** Toggles (hides) the right-hand side Details Pane.
* **Guide** Link to the corresponding User Guide
* **Download:**  Downloads the selected item.
* **View** Displays the content of the file, typically as plain text or rendered html, depending on filetype.
* **Delete** Deletes the file.
* **Rename** Allows renaming of the file.
* **Copy:** Copies the selected items to the clipboard.
* **Move** Allows moving of the file to another folder.
* **Edit Type** Allows changing of the type of the file in terms of how PATRIC interprets the content and uses it in other services or parts of the website.  Allowable types include unspecified, contigs, nwk, reads, differential expression input data, and differential expression input metadata. Only files in this same set can be retyped. The type for html and text files cannot be changed.

More details are available in the [Action Buttons](../other/action_buttons.html) user guide.


## References
 * Ondov BD, Bergman NH, and Phillippy AM. Interactive metagenomic visualization in a Web browser. BMC Bioinformatics. 2011 Sep 30; 12(1):385.
 * Maidak, Bonnie L., et al. "The RDP (ribosomal database project)." Nucleic acids research 25.1 (1997): 109-110.
 * Wood DE, Salzberg SL: Kraken: ultrafast metagenomic sequence classification using exact alignments. Genome Biology 2014, 15:R46.
 * Yilmaz P, Parfrey LW, Yarza P, Gerken J, Pruesse E, Quast C, Schweer T, Peplies J, Ludwig W, Glöckner FO. The SILVA and “All-species Living Tree Project (LTP)” taxonomic frameworks. Nucleic Acids Res. 2014; 42(Database issue):643–8.
 
 
