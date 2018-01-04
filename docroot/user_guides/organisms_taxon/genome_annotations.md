# Genome Annotations

## Annotation sources

PATRIC provides two basic annotation sources, RefSeq, and PATRIC. RefSeq sequences from NCBI, have each been annotated by the submitting researcher using methodologies of their choice. PATRIC re-annotates all genomes using RAST tool kit [(RASTtk)](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4322359/) to provide annotation consistency across a wide variety of genomes. The
original RefSeq annotations have been retained and are still available for comparison purposes.

Genomes that are in more than 500 contigs are not annotated by RAST. Nor are plasmid-only genomes. There is approximately a two-month interval between when sequences are submitted to RefSeq and re-annotation/integration with PATRIC, thus there may be a significant difference in the number of genomes at NCBI and at PATRIC.

## Annotated Features
Currently, PATRIC supports the following genomic feature types:

* -10_signal
* -35_signal
* 5’UTR
* attenuator
* CDS
* conflict
* enhancer
* exon
* gene
* intron
* LTR
* mat_peptide
* misc_binding
* misc_difference
* misc_feature
* misc_recomb
* misc_RNA
* misc_signal
* misc_structure
* mRNA
* ncRNA
* old_sequence
* prim_transcript
* primer_bind
* promoter
* protein_bind
* pseudogene
* pseudogenic_region
* RBS
* region
* rep_origin
* repeat_region
* repeat_unit
* ribosome_entry_site
* rRNA
* sig_peptide
* source
* stem_loop
* terminator
* tmRNA
* transcript
* tRNA
* unsure
* variation
