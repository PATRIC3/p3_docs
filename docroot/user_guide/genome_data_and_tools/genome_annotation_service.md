# Genome Annotation Service

## Overview
The Genome Annotation Service uses the RAST tool kit (RASTtk) to provide annotation of genomic features. Once the annotation process has started by clicking the Annotate button, the genome is queued as a “job” for the Annotation Service to process, and will increment the count in the Jobs information box on the bottom right of the page. Once the annotation job has successfully completed, the output file will appear in the workspace, available for use in the PATRIC comparative tools and downloaded if desired. A tutorial for using the Annotation Service is available here.

The Genome Annotation Service can be accessed from the Services Menu at the top of the PATRIC website page. RASTtk also accommodates the batch submission of genomes and the ability to customize annotation protocols for batch submissions, available via the PATRIC Command Line Interface (CLI).

## Taxon information
Taxon must be specified at the genus level or below to get the latest
protein family predictions.

## How-to

How-to information and details concerning the annotation service can be
found
[here](http://enews.patricbrc.org/faqs/genome-annotation-service/).

## Parameters

**Contigs** The target FASTA file containing the genome sequence to
annotate.

**Organism Name** Type or select an organism name. If the target species
or strain is not listed select the most specific, accurate taxonomic
level available.

**Genetic Code** The codon translation used in calling genes.

**Domain** The taxonomic domain of the target organism: bacteria or
archaea.

**Output Folder** The workspace folder where results will be placed.
