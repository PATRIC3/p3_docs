# Similar Genome Finder Service

## Overview
The Similar Genome Finder Service will find similar public genomes in PATRIC or compute genome distance estimation using [Mash/MinHash](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4915045/). It returns a set of genomes matching the specified similarity criteria. 

### See also
* [Similar Genome Finder Service](https://patricbrc.org/app/GenomeDistance)
* [Similar Genome Finder Service Tutorial](https://docs.patricbrc.org//tutorial/similar_genome_finder/similar_genome_finder.html)

## Using the Similar Genome Finder Service
The **Similar Genome Finder** submenu option under the **Services** main menu (Genomics category) opens the Similar Genome Finder input form (*shown below*).

![Similar Genome Finder Menu](../images/services_menu.png)

![Similar Genome Finder Input Form](../images/similar_genome_finder_input_form.png)

## Select a Genome
Specifies the genome to use as the basis for finding other similar genomes

### Search by Genome Name or Genome ID
Selection box for specifying genome in PATRIC to use as the basis of comparison

### Or Upload FASTA
Alternate option for uploading a FASTA file to use as the basis of comparison. *Note: You must be logged into PATRIC to use this option.* 

## Advanced Options

### Parameters

**Max Hits:** The maximum number of matching genomes to return. 

**P-Value Threshold:** Sets the maximum allowable p-value associated with the [Mash](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4915045/) Jaccard estimate used in calculating the distance.

**Distance:**  Mash distance, which estimates the rate of sequence mutation under as simple evolutionary model using k-mers. The Distance parameter sets the maximum Mash distance to include in the Similar Genome Finder Service results. Mash distances are probabilistic estimates associated with p-values. 

**Scope:** Option for limiting the search to only Reference and Representative genomes, or all genomes in PATRIC.

## Buttons

**Search:** Launches the similar genome finder job.
