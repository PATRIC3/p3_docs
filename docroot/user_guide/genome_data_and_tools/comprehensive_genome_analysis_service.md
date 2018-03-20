# Comprehensive Genome Analysis Service (DRAFT)

## Overview

The Comprehensive Genome Analysis Service allows ...

When starting with read file, ..., below is copied from Genome Assembly Service: allows single or multiple assemblers to be invoked to compare results. The service attempts to select the best assembly, i.e., assembly with the smallest number of contigs and the longest average contig length. Several assembly workflows or “recipes” are available that have been tuned to fit certain data types or desired analysis criteria such as throughput or rigor. Once the assembly process has started by clicking the Assemble button, the genome is queued as a “job” for the Assembly Service to process, and will increment the count in the Jobs information box on the bottom right of the page. Once the assembly job has successfully completed, the output file will appear in the workspace, available for use in the PATRIC comparative tools and downloaded if desired. A tutorial for using the Assembly Service is available here.

When starting with assembled contigs file, ..., The Genome Annotation Service uses the RAST tool kit (RASTtk) to provide annotation of genomic features. Once the annotation process has started by clicking the Annotate button, the genome is queued as a “job” for the Annotation Service to process, and will increment the count in the Jobs information box on the bottom right of the page. Once the annotation job has successfully completed, the output file will appear in the workspace, available for use in the PATRIC comparative tools and downloaded if desired. A tutorial for using the Annotation Service is available here.

The Comprehensive Genome Analysis Service can be accessed from the Services Menu at the top of the PATRIC website page.

## Start with
Start with text goes here.

## Selected libraries
Read files placed here will contribute to a single assembly.

## Read Input File
(TEXT needs proof read). You can provide read file in paired read library, single read library or SRA run accession. For paired read library, many paired read libraries are given as file pairs, with each file containing half of each read pair. Paired read files are expected to be sorted such that each read in a pair occurs in the same Nth position as its mate in their respective files. These files are specified as READ FILE 1 and READ FILE 2. For a given file pair, the selection of which file is READ 1 and which is READ 2 does not matter.

## Parameters

### Assembly Strategy
ONLY when you choose to start with read file.

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

### Contigs
The target FASTA file containing the genome sequence to annotate.

### Domain
The taxonomic domain of the target organism: bacteria or archaea.

### Taxon information
Taxon must be specified at the genus level or below to get the latest
protein family predictions.

### Organism Name
Type or select an organism name. If the target species or strain is not listed
select the most specific, accurate taxonomic level available.

### Genetic Code
The codon translation used in calling genes.

### Output Folder
The workspace folder where results will be placed.

### Output Name
Name used to uniquely identify results.
