# Genome Annotation Service

## Overview
The Genome Annotation Service uses the RAST tool kit, [RASTtk](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4322359/), to provide annotation of genomic features. Once the annotation process has started by clicking the Annotate button, the genome is queued as a "job" for the Annotation Service to process, and will increment the count in the Jobs information box on the bottom right of the page. Once the annotation job has successfully completed, the output file will appear in the workspace, available for use in the PATRIC comparative tools and downloaded if desired.

### See also
* [Genome Annotation Service](https://patricbrc.org/app/Annotation)
* [Genome Annotation Service Tutorial](https://docs.patricbrc.org/tutorial/genome_annotation/annotation.html)

## Using the Genome Annotation Service
The **Annotation** submenu option under the **Services** main menu (Genomics category) opens the Genome Annotation input form (*shown below*). *Note: You must be logged into PATRIC to use this service.*

![Annotation Menu](../images/services_menu.png)

*Note:* RASTtk also accommodates the batch submission of genomes and the ability to customize annotation protocols for batch submissions, available via the PATRIC Command Line Interface (CLI).

![Annotation Input Form](../images/annotation_input_form.png)

## Parameters

**Contigs:** The target FASTA file containing the genome sequence to annotate.

**Domain** The taxonomic domain of the target organism: bacteria or
archaea.

**Taxonomy Name:** The user-entered or selected taxonomic name for the organism. If the target species or strain is not listed, select the most specific, accurate taxonomic level available. 

**My Label:** The user-provided name to identify the annotation result.

**Output Name:** The taxonomy name concatenated with the chosen label.  This name will appear in the workspace when the annotation job is complete.

**Genetic Code:** The codon translation used in calling genes.

**Output Folder:** The workspace folder where results will be placed.

## Taxon information
Taxon must be specified at the genus level or below to get the latest
protein family predictions.

## Buttons

**Reset:** Resets the input form to default values

**Annotate:** Launches the annotation job.

6. A message will appear below the box to indicate that the job is now in the queue.

    ![Step 17](./images/image17.png "Step 17")

## Job Launch
Clicking on the Jobs indicator at the bottom of the PATRIC page open the Jobs Status page that displays all current and previous service jobs and their status. 

    ![Step 18](./images/image18.png "Step 18")

2. This will 

    ![Step 19](./images/image19.png "Step 19")

3. Once the job is completed, you can select the job by clicking on it and click the "View"
button on the right-hand bar to see the results.

    ![Step 20](./images/image20.png "Step 20")

4. The results page will consist of a header describing the job and a list of output files,
as shown below.

    ![Step 21](./images/image21.png "Step 21")

5. The first file is *GenomeReport.html*, which is described in [Analyzing Genome Quality](/tutorial/genome_quality_report/genome_quality_report.html).
This file contains a link to the genome's pages in the PATRIC Genome Browser as well as
information about the general quality of the genome. The remaining files shown are as
follows.

*   **contigs.fasta** contains the assembled contigs of the genome in DNA FASTA format.
*   **embl** contains an EMBL dump of the annotated genome.
*   **feature_dna.fasta** contains all the feature sequences of the genome in DNA FASTA format.
*   **feature_protein.fasta** contains all the protein sequences of the genome in protein
    FASTA format.
*   **features.txt** is a tab-delimited text file listing all the features of the genome.
    For each feature, it contains the PATRIC ID, the location string, the feature type,
    the functional assignment, any alternated IDs found, and (for protein-coding genes)
    the protein MD5 checksum.
*   **gb** contains the annotated genome in GENBANK format.
*   **genome** contains a special "Genome Typed Object (GTO)" JSON-format file that encapsulates all the data from the annotated genome. See [Extracting and Mining Genome Typed Objects](https://docs.patricbrc.org/cli_tutorial/cli_getting_started.html#extracting-and-mining-genome-typed-objects-gtos) for more information.
*   **gff** lists all the features of the genome in General Feature Format.


## References

1. Wattam AR, Davis JJ, Assaf R, Boisvert S, Brettin T, Bun C, Conrad N, Dietrich EM, Disz T, Gabbard JL, Gerdes S, Henry CS, Kenyon RW, Machi D, Mao C, Nordberg EK, Olsen GJ, Murphy-Olson DE, Olson R, Overbeek R, Parrello B, Pusch GD, Shukla M, Vonstein V, Warren A, Xia F, Yoo H, Stevens RL. (2017) Improvements to PATRIC, the all-bacterial Bioinformatics Database and Analysis Resource Center. Nucleic Acids Res. 45(D1): D535-D542.

2. Brettin T, Davis JJ, Disz T, Edwards RA, Gerdes S, Olsen GJ, Olson R, Overbeek R, Parrello B, Pusch GD, Shukla M, Thomason JA 3rd, Stevens R, Vonstein V, Wattam AR, Xia F. (2015). RASTtk: a modular and extensible implementation of the RAST algorithm for building custom annotation pipelines and annotating batches of genomes. Scientific reports 5: 8365.


