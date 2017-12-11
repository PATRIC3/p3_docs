========================================================================================================================================================================================================
PATRIC June 2015 Release Features Integrated Comparative Analysis Capabilities with User-Supplied Genomes and New Services for Protein-Based Genome Comparison, RNA-Seq Analysis, and Metabolic Modeling
========================================================================================================================================================================================================


:date:   2015-06-16T15:41:52+00:00

The June Release delivers the second stage of genome assembly,
annotation and integrated analysis in PATRIC. It also includes a new
Proteome Comparison Service, RNA-Seq Analysis Service, and Metabolic
Modeling Service, plus updates to the Private Workspace and other
enhancements.

***NOTE: You must have a PATRIC user account and be logged-in to use the
services and workspace.***

**Integrated Genome Comparative Analysis Capability**

With this release, users can now view their private genome annotated
with the PATRIC `Genome Annotation
Service <https://www.patricbrc.org/app/Annotation>`__ in the context of
all of the public genomes in PATRIC. This includes the ability to use
all of the PATRIC genome presentation and comparative tools such as the
Genome Browser, Gene Page, Protein Family Sorter, Comparative Pathway
Analysis Service, and Global Search. The user’s genome is visible only
to the user, and only if they are logged into PATRIC.

**Proteome Comparison Service**

The Proteome Comparison Service performs protein sequence-based genome
comparison using bidirectional blastp. This service allows users to
select up to 8 genomes (either public or private) and compare them to a
user selected reference genome. The service also allows users to upload
an external genome file in FASTA format for an additional comparison.
The genome comparison result is displayed as a Circos genome view on the
webpage. Both the SVG image and the bidirectional blastp comparison
result can be downloaded. The Proteome Comparison Service can be
accessed at https://www.patricbrc.org/app/SeqComparison.

**Metabolic Modeling Service**

With the release of the Metabolic Modeling Service, users can construct
their own metabolic model for any genome in PATRIC. The service includes
support for model gap-filling, flux balance analysis, essential gene
prediction, and export of models in SBML format. The Metabolic Modeling
Service leverages capabilities of the ModelSEED (`PMID:
20802497 <http://www.ncbi.nlm.nih.gov/pubmed/20802497>`__) and is
available in PATRIC at https://www.patricbrc.org/app/Reconstruct.

**RNA-Seq Analysis Service**

PATRIC is now providing services for aligning, assembling, and testing
differential expression on RNA-Seq data. The new service provides two
recipes for processing RNA-Seq data: 1) Rockhopper, based on the popular
`Rockhopper <http://www.genomebiology.com/2015/16/1/1/abstract>`__ tool
for processing prokaryotic RNA-Seq data; and 2) Tuxedo, based on the
`tuxedo suite of
tools <http://www.nature.com/nprot/journal/v7/n3/full/nprot.2012.016.html>`__
(i.e., Bowtie, Cufflinks, Cuffdiff). The new tool provides SAM/BAM
output for alignment, tab delimited files profiling expression levels,
and differential expression test results between conditions. Look for
more integration of the resulting RNA-Seq analysis data in coming
months. The PATRIC RNA-Seq Analysis Service can be accessed at
https://www.patricbrc.org/app/Rnaseq.
