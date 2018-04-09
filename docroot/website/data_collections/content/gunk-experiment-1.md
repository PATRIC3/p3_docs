
# Resources for Genetic and Genomic Analysis of Emerging Pathogen Acinetobacter baumannii

**Publication:** [PMC4438207](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4438207/)

Acinetobacter baumannii is a Gram-negative bacterial pathogen notorious for causing serious nosocomial infections that resist antibiotic therapy. Research to identify factors responsible for the pathogen’s success has been limited by the resources available for genome-scale experimental studies. This report describes the development of several such resources for A. baumannii strain AB5075, a recently characterized wound isolate that is multidrug resistant and displays robust virulence in animal models. We report the completion and annotation of the genome sequence, the construction of a comprehensive ordered transposon mutant library, the extension of high-coverage transposon mutant pool sequencing (Tn-seq) to the strain, and the identification of the genes essential for growth on nutrient-rich agar. These resources should facilitate large-scale genetic analysis of virulence, resistance, and other clinically relevant traits that make A. baumannii a formidable public health threat.

## Comprehensive Ordered Transposon Mutant Library

As a resource for genetic analysis of AB5075, we created an arrayed library of mutants with defined transposon insertions in most nonessential genes of the organism. Our goal was to create a colony-purified library with relatively complete genome coverage that was small enough to facilitate efficient phenotype screening. We also wanted it to include several different mutations for each gene to minimize missed genotype-phenotype associations arising from noninactivating mutations or library cross-contamination and to provide immediate confirmation of associations observed. To meet these objectives, we created a library made up of two to three different insertion mutants per nonessential gene.

**Conditions:**  Growth on TYE agar of individual transposon insertion mutants as described in paper.
**Library:**  Comprehensive arrayed library of individual, sequence-defined transposon insertion mutants. This library serves as a curated source of individually-retrievable mutant strains.
Transposon used:  T26 (Tn5-based, encoding tetracycline resistance, bearing LoxP sites flanking the resistance marker to facilitate marker recycling).
**Protocol for library preparation:**  Electroporation of transposon-transposase complexes, followed by picking, arraying, storage and sequencing of individual mutants, as described in paper.  Second “three-allele” arrayed library was generated from the primary library by cherry-picking three mutant strains per gene.
**Protocol for sequencing:**  Transposon-genome junctions from individual strains were amplified and sequenced by Sanger sequencing.
Protocol for data processing:  custom sequence-read parsing and mapping scripts which call crossmatch for mapping.
**Reference Genome:** Acinetobacter baumannii AB5075-UW
**Experimenter/Researcher/Owner of Data:** Colin Manoil, University of Washington
**PI/Lab:** Colin Manoil, University of Washington
**Uploaded/Deposited by:** Larry Gallagher, University of Washington
**Dataset:** [Supplemental file S1](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4438207/bin/supp_197_12_2027__index.html)

## Tn-seq Analysis of Acinetobacter baumannii AB5075

To provide an efficient procedure for screening pools of mutants for genotype-phenotype associations, we extended transposon insertion pool screening (Tn-seq) to AB5075. We used transposon Tn5-based methodology to provide high genome coverage. We compared two different Tn-seq procedures, the circle method we developed and an adaptation to Tn5 of a method that utilizes terminal deoxynucleotidyl transferase (TdT). Approximately 450,000 T26 insertion mutants selected on LB agar were pooled, and DNA from the pool was analyzed by the two methods. Both methods successfully identified insertions comparable in number to the predicted pool complexity. The two Tn-seq methods both worked well for A. baumannii AB5075 and provided remarkably similar lists of essential genes.

**Conditions:** Growth on TYE agar and pooling of individual transposon insertion mutants as described in paper.
**Library:** Pool of approximately 450,000 mutants.
**Transposon used:** T26 (Tn5-based, encoding tetracycline resistance, bearing LoxP sites flanking the resistance marker to facilitate marker recycling).
**Protocol for library preparation:**  Electroporation of transposon-transposase complexes, followed by pooling of individual mutants, as described in paper.
**Protocol for TnSeq sample preparation:**  Two methods were used and compared, the circle method and the TdT method.
**Protocol for sequencing:** 50-bp single-end reads on Illumina MiSeq.
**Protocol for data processing:**  custom Tn-seq data processing scripts which map reads using BWA, then count reads per insertion site and normalize as described in paper.
**Reference Genome:** Acinetobacter baumannii AB5075-UW
**Experimenter/Researcher/Owner of Data:** Colin Manoil, University of Washington
**PI/Lab:** Colin Manoil, University of Washington
**Uploaded/Deposited by:** Larry Gallagher, University of Washington

**Datasets:** TBD

## Candidate Essential Genes

The transposon insertion profiles from Tn-seq and the primary ordered mutant library represent independent data sets that can be used to identify AB5075 genes essential for growth on nutrient-rich agar. The data sets reflect complementary advantages and disadvantages of the two procedures for identifying essential genes. The Tn-seq analysis provides high genome coverage but does not distinguish well between slow-growing and nongrowing mutants because the strains in the pool are grown in competition. The ordered library was generated from isolated colonies and should include slow-growing mutants but provides lower genome coverage and is therefore expected to lack insertions by chance in more nonessential genes than Tn-seq analysis. We therefore defined candidate essential genes as those with low representation in both data sets (see Fig. S3A to C in the supplemental material). The 438 candidate essential genes are listed in Data Set S2 in the supplemental material.

**Dataset:** [Supplemental file S2](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4438207/bin/supp_197_12_2027__index.html)

