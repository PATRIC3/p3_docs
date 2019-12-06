# Genome Assembly Service (Revised Service Dec 2019)

## Overview
The Genome Assembly Service allows single or multiple assemblers to be invoked to compare results. The service attempts to select the best assembly, i.e., assembly with the smallest number of contigs and the longest average contig length. Several assembly workflows or "recipes" are available that have been tuned to fit certain data types or desired analysis criteria such as throughput or rigor. Once the assembly process has started by clicking the Assemble button, the genome is queued as a "job" for the Assembly Service to process, and will increment the count in the Jobs information box on the bottom right of the page. Once the assembly job has successfully completed, the output file will appear in the workspace, available for use in the PATRIC comparative tools and downloaded if desired.

### See also
* [Genome Assembly Service](https://patricbrc.org/app/Assembly2)
* [Genome Assembly Service Tutorial](https://docs.patricbrc.org/tutorial/genome_assembly/assembly2.html)

## Using the Genome Assembly Service
The **Assembly** submenu option under the **Services** main menu (Genomics category) opens the Genome Assembly input form (*shown below*). *Note: You must be logged into PATRIC to use this service.*

![Assembly Menu](../images/services_menu.png)

## Options
![Assembly Input Form](../images/assembly2_input_form.png) 

## Selected libraries
Read files placed here will contribute to a single assembly.

## Paired read library

**Read File 1 & 2:**  Many paired read libraries are given as file pairs, with each file containing half of each read pair. Paired read files are expected to be sorted such that each read in a pair occurs in the same Nth position as its mate in their respective files. These files are specified as READ FILE 1 and READ FILE 2. For a given file pair, the selection of which file is READ 1 and which is READ 2 does not matter.

**Advanced:**
  * File 1 Interleaved - Some paired libraries are available in a single file where each read in a pair occurs in succession. To specify such a file set this parameter to 'True'.

  * Mean Insert Size - This refers to the mean insert size between paired reads. If you have this information you may provide it. If not the assembly algorithm will make an attempt to determine this value.
  
  * Std. Insert Size - This refers to the standard deviation of the insert size between paired reads. If you have this information you may provide it. If not the assembly algorithm will make an attempt to determine this value.
  
  * Mate Paired- Defines the orientation of read pairs. Setting Mate Paired to true indicates that the sequencing direction of the two reads in each pair is outward facing.
  
  * Platform - The sequencing platform used for each library.
    * infer: Infer sequencing platform from read files
    * illumina: Illumina short reads
    * pacbio: PacBio long reads
    * nanopore: MinION long reads

## Single read library

**Read File:**
The fastq file containing the reads

**Advanced:**

  * Platform - The sequencing platform used for each library.
    * infer: Infer sequencing platform from read files
    * illumina: Illumina short reads
    * pacbio: PacBio long reads
    * nanopore: MinION long reads

## SRA run accession
Allows direct upload of read files from the [NCBI Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) to the PATRIC Assembly Service. Entering the SRR accession number and clicking the arrow will add the file to the selected libraries box for use in the assembly. 

## Parameters

**Assembly Strategy:**
  * auto
    * For short reads:
      1. Runs BayesHammer on reads
      2. Assembles with Velvet, IDBA and SPAdes
      3. Sorts assemblies by ARAST quality score

    * For long reads (PacBio or Nanopore):
      1. Assembles with MiniASM

  * fast
    1. Assembles with MEGAHIT and Velvet.
    2. Results are sorted by ARAST quality score.

  * full_spades
    1. Runs BayesHammer on reads
    2. Assembles with SPAdes.

  * kiki
    1. Runs the Kiki assembler

  * miseq
    1. Runs Velvet with hash length 35.
    2. Runs BayesHammer on reads and assembles with SPAdes with k up to 99.
    3. Results are sorted by ARAST quality score.
    4. Works for Illumina MiSeq reads.

  * plasmid
    1. Runs BayesHammer on reads and assembles with plasmidSPAdes.

  * smart
    * For short reads:
      1. Runs BayesHammer on reads, Kmergenie to choose hash-length for Velvet
      2. Assembles with Velvet, IDBA and SPAdes
      3. Sorts assemblies by ALE score
      4. Merges the two best assemblies with GAM-NGS

    * For long reads (PacBio or Nanopore):
      1. Assembles with MiniASM

**Output Folder:** The workspace folder where results will be placed.

**Output Name:** User-provided name used to uniquely identify results.

**Benchmark Contigs:** This optional parameter can be used to specify a FASTA contigs file to evaluate the assembly against.

## Advanced

**Minimal output contig length:**  Filter out short contigs in final assembly

**Minimal output contig coverage:** Filter out contigs with low read depth in final assembly

### Assembly Pipeline
The pipeline parameter is an advanced way to customize the assembly workflow by mixing and matching a variety of modules. Each modules works at one of the three stages of the pipeline: preprocessing, assembly, and post-processing. In general, you can compose a pipeline by concating one or more preprocessing modules, one assembler, and optionally one
postprocessor.

**Example 1: tagdust velvet** This pipeline will simply run tagdust to remove adapter sequences in the reads and then assemble them with velvet. Note: quotes should not be used around the two modules as they have special meaning in pipeline syntax.

**Example 2: a6**  You can also invoke an assembler that we have not included in our curated strategies. In this case, A6 is an assembler with its built-in preprocessing and postprocessing steps.

**Example 3: "tagdust none" "megahit velvet" sspace**  You can use quotes to specify alternative modules you would like to try at each step. This example will launch a cartesian combination of four parallel pipelines: tagdust+megahit+sspace, tagdust+velvet+sspace, megahit+sspace, velvet+sspace.

*Note:* The pipeline parameter overrides the assembly strategy parameter. Not all modules combine well.
[List of modules supported](https://github.com/PATRIC3/p3_docs/blob/master/docroot/user_guides/services/arast_supported_modules.txt).

## Buttons

**Reset:** Clicking this button resets the input form to default values

**Assemble:** Clicking this button launches the assembly job.

## Output Results
![Assembly Service Output Files](../images/genome_assembly_output_files.png) 

The Genome Assembly Service generates several files that are deposited in the Private Workspace in the designated Output Folder. These include

* **strategy_contigs.fasta** - A FASTA file containing the contigs generated by the selected assembly strategy.
* **analysis.zip** - A zip file containing results of QUAST (Quality Assessment Tool for Genome Assemblies) for the assembly.
* **contigs.fa** - File containig contigs for best assembly
* **report.txt** - Text file providing details of the assembly process.

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
* **Edit Type** Allows changing of the type of the file in terms of how PATRIC interprets the content and uses it in other services or parts of the website.  Allowable types include unspecified, contigs, nwk, reads, differential expression input data, and differential expression input metadata.

More details are available in the [Action Buttons](../action_buttons.html) user guide.

## References
1. Branton, D., et al., The poten al and challenges of nanopore sequencing. Nature biotechnology, 2008. 26(10): p. 1146‑1153.
2. Nikolenko, S.I., A.I. Korobeynikov, and M.A. Alekseyev, BayesHammer: Bayesian clustering for error correc on in single‑cell sequencing. BMC genomics, 2013. 14(1): p. 1.
3. Zerbino, D.R. and E. Birney, Velvet: algorithms for de novo short read assembly using de Bruijn graphs. Genome research, 2008. 18(5): p. 821‑829.
4. Peng, Y., et al. IDBA: a prac cal itera ve de Bruijn graph de novo assembler. in Research in Computa onal Molecular Biology. 2010. Springer.
5. Bankevich, A., et al., SPAdes: a new genome assembly algorithm and its applica ons to single‑cell sequencing. Journal of Computational Biology, 2012. 19(5): p. 455‑477.
6. Li, D., et al., MEGAHIT: an ultra‑fast single‑node solu on for large and complex metagenomics assembly via succinct de Bruijn graph. Bioinforma cs, 2015: p. btv033.
7. An pov D, Hartwick N, Shen M, Raiko M, Lapidus A, Pevzner PA. 2016. plasmidSPAdes: assembling plasmids from whole genome sequencing data. Bioinforma cs32(22):3390‑3397.
8. Namiki, T., et al., MetaVelvet: an extension of Velvet assembler to de novo metagenome assembly from short sequence reads. Nucleic acids research, 2012. 40(20): p. e155‑e155.
9. Clark, S.C., et al., ALE: a generic assembly likelihood evalua on framework for assessing the accuracy of genome and metagenome assemblies. Bioinforma cs, 2013: p. bts723.
10. Vicedomini, R., et al., GAM‑NGS: genomic assemblies merger for next genera on sequencing. BMC bioinforma cs, 2013. 14(7): p. 1.
11. Li, H., Minimap and miniasm: fast mapping and de novo assembly for noisy long sequences. arXiv preprint arXiv:1512.01801, 2015.
12. Gurevich, A., et al., QUAST: quality assessment tool for genome assemblies. Bioinforma cs, 2013. 29(8): p. 1072‑1075.
