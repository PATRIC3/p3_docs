# Taxonomic Classification Service

## Overview
The Taxonomic Classification Service accepts reads or contigs from sequencing of a metagenomic sample and uses Kraken to assign the reads to taxonomic bins, providing an initial profile of the possible constituent organisms present in the sample.

### See also
  * [Taxonomic Classification Service](https://patricbrc.org/app/TaxonomicClassification)
  * Taxonomic Classification Service Tutorial - TBD
  * [Metagenome Binning Service](./metagenome_binning_service.html)

## Using the Taxonomic Classification Service
The **Taxonomic Classification** submenu option under the **Services** main menu (Metagenomics category) opens the Taxonomic Classification input form (shown below). *Note: You must be logged into PATRIC to use this service.*

![Taxonomic Classification Menu](../images/services_menu.png)

## Options
![Taxonomic Classification Input Form](../images/taxonomic_classification_input_form.png)

WORK IN PROGRESS - GOT TO HERE

## Start with
The service can accept either read files or assembled contigs. If the "Read Files" option is selected, the Assembly Service will be invoked automatically to assemble the reads into contigs before invoking the Annotation Service. If the "Assembled Contigs" option is chosen, the Annotation Service will automatically be invoked, bypassing the Assembly Service.

## Read Input File
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

### Assembly Strategy
*Note: Available only when "Read File" is selected above.*

#### auto
  * For short reads:
    1. Runs BayesHammer on reads
    2. Assembles with Velvet, IDBA and SPAdes
    3. Sorts assemblies by ARAST quality score

  * For long reads (PacBio or Nanopore):
    1. Assembles with MiniASM

#### fast
  1. Assembles with MEGAHIT and Velvet.
  2. Results are sorted by ARAST quality score.

#### full_spades
1. Runs BayesHammer on reads
2. Assembles with SPAdes.

#### kiki
1. Runs the Kiki assembler

#### miseq
1. Runs Velvet with hash length 35.
2. Runs BayesHammer on reads and assembles with SPAdes with k up to 99.
3. Results are sorted by ARAST quality score.
4. Works for Illumina MiSeq reads.

#### plasmid
1. Runs BayesHammer on reads and assembles with plasmidSPAdes.

#### smart
- For short reads:
  1. Runs BayesHammer on reads, Kmergenie to choose hash-length for Velvet
  2. Assembles with Velvet, IDBA and SPAdes
  3. Sorts assemblies by ALE score
  4. Merges the two best assemblies with GAM-NGS

- For long reads (PacBio or Nanopore):
  1. Assembles with MiniASM

### Domain
The taxonomic domain of the target organism: bacteria or archaea.

### Taxonomy Name
Taxon must be specified at the genus level or below to get the latest
protein family predictions.

### Taxonomy ID
Auto-populated after entering Taxonomy Name. If a Taxonomy ID is entered, auto-populates the Taxonomy Name

### Genetic Code
The codon translation used in calling genes.

### Output Folder
The workspace folder where results will be placed.

### Output Name
Name used to uniquely identify results.

## Output Results
![Comprehensive Genome Analysis Output Files](../images/cga_service_output_files.png)

The Comprehensive Genome Analysis Service generates several files that are deposited in the Private Workspace in the designated Output Folder. These include

 * **FullGenomeReport.html** - A web-browser-viewable report that summarizes the results of the service including
   * Summary information - genome name, quality,
   * Genome assembly information - contigs, GC content, plasmids, L50, genome length, chromosomes
   * Genome annotation information - taxonomy, CDS, tRNA, rRNA, partial CDS, misc RNA, repeat regions, protein feature summary, circular view with annotations
   * Specialty genes - antibiotic resistance, drug targets, transporters, virulence factors
   * Subsystem analysis - summary
   * Phylogenetic analysis - phylogenetic tree generated using the analyzed genome and the closest Reference and Representative genomes
   * References - citations to all tools used by the service
 * **annotated.genome** - A special "Genome Typed Object (GTO)" JSON-format file that encapsulates all the data from the annotated genome. See [Extracting and Mining Genome Typed Objects](https://docs.patricbrc.org/cli_tutorial/cli_getting_started.html#extracting-and-mining-genome-typed-objects-gtos) for more information.
 * **annotation** - The Annotation sub-job that was run as part of the CGA Service. Double-clicking this item will display the Annotation job results. Note that sub-jobs are indicated by the "checkered flag" icon beside the name.
 * **assembly** - The Assembly sub-job that was run as part of the CGA Service. Double-clicking this item will display the Assembly job results. Note that sub-jobs are indicated by the "checkered flag" icon beside the name.
 * **circos.svg** - SVG-format rendering of the circular genome view used in the FullGenomeReport.html file.
 * **circos.png** - PNG-format rendering of the circular genome view used in the FullGenomeReport.html file.
 * **codonTree.nex** - NEXUS-format file containing the phylogenetic tree generated by the CGA Service.
 * **codonTree.nwk** - Newick-format file containing the phylogenetic tree generated by the CGA Service.
 * **codonTree.stats** - File containing the statistics on the phylogenetic tree generated by the CGA Service.
 * **codonTree.svg** - SVG-format rendering of the phylogenetic tree used in the FullGenomeReport.html file.
 * **subsystem_colors.json** - JSON-format file used for rendering colors in the Subsystem pie chart displayed in the FullGenomeReport.html file.
 * **tree_ingroup.txt** - File containing the closely related genomes used in building the ingroup for the phylogenetic tree generated by the CGA Service.
