:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/20160405-patric-march-2016-release-features-a-new-variation-analysis-service-annotation-and-proteome-comparison-service-enhancements-curated-amr-related-genes-new-data-from-functional-genomics-and-systems-b.rst

============================================================================================================================================
PATRIC March 2016 Release Features a New Variation Analysis Service, Service Enhancements, New AMR and other Data, and over 9000 New Genomes
============================================================================================================================================

.. feed-entry::
   :date: 2016-04-05

*NOTE: You must have a PATRIC user account and be logged in to use the
services and workspace.*

**Variation Analysis Service**

The new Variation Service can be used to identify and annotate sequence
variations. The service enables users to upload one or multiple short
read samples and compare them to a closely related reference genome. For
each sample, the service computes the variations against the reference
and presents a detailed list of SNPs, MNPs, insertions and deletions
with confidence scores and effects such as “synonymous mutation” and
“frameshift”. High confidence variations are downloadable in the
standard VCF format augmented by SNP annotation. A summary table
illustrating how the variations are shared across the samples is also
available. The PATRIC Variation Service can be accessed at
https://www.patricbrc.org/app/Variation.

**Annotation Service Enhancements**

The PATRIC Genome Annotation Service now includes an AMR classifier
module built into RASTtk that performs species-specific AMR phenotype
and genomic feature prediction. This classifier was built using PATRIC’s
collection of genomes, binned by AMR phenotype along with metadata
including minimum inhibitory concentrations (MICs). From this, we custom
built AdaBoost (adaptive boosting) machine learning classifiers for
identifying carbapenem resistance in *Acinetobacter baumannii*,
methicillin resistance in *Staphylococcus aureus*, and beta-lactam and
co-trimoxazole resistance in *Streptococcus pneumonia.* We also did this
for isoniazid, kanamycin, ofloxacin, rifampicin, and streptomycin
resistance in *Mycobacterium tuberculosis*. A corresponding manuscript
has been submitted. The PATRIC Genome Annotation Service can be accessed
at https://www.patricbrc.org/app/Annotation.

**Proteome Comparison Service Enhancements**

PATRIC’s Proteome Comparison Service now allows users to select a public
or a private genome in PATRIC as a reference genome, as well as a
user-supplied FASTA file or saved feature group as the reference. The
service now also supports selection of multiple FASTA files and/or
feature groups for comparison. The PATRIC Proteome Comparison Service
can be accessed at https://www.patricbrc.org/app/SeqComparison.

**Curated Antimicrobial Resistance (AMR) Genes**

PATRIC has undertaken an antimicrobial resistance (AMR) curation effort
with the goal of providing PATRIC users with the ability to rapidly
recognize and project known AMR related genome features to new genomes
in an automated fashion and to use comparative genomics approaches for
the discovery of new resistance mechanisms. Curation thus far has
focused on encoding the following mechanisms of drug resistance: outer
membrane porins, multidrug efflux mechanisms, and capsular and
extracellular polysaccharides. To date, we have encoded 25 subsystems
covering 265 unique functional roles (protein families). Additional
information and curated data are available
`here <http://enews.patricbrc.org/4974/patric-antimicrobial-resistance-amr-gene-curation/>`__.

**Changes to the FTP Site**

We have completed reorganization and updating of the PATRIC FTP site. It
now contains downloadable updated FTP files for all PATRIC
protein-protein interaction data, available from
ftp://ftp.patricbrc.org/patric2/ppi/.

**New Genomes, Annotations, and Other Data**

In this release, 9280 new genomes have been added to PATRIC, bringing
the total to over 67,000. Approximately 4600 of these genomes are from
the Sanger Center and are part of large-scale sequencing projects. This
release also included 173 *Staphylococcus* and *Streptococcus* genomes
with AMR and clinical metadata from a PATRIC collaboration. We have also
updated the list of reference and representative genomes based on the
latest NCBI and Uniprot Reference genome sets. The genomes labeled as
ref/rep at PATRIC before, are still labeled as such. Also included are
additional curated AMR metadata from NIAID Genomics Centers for
Infectious Diseases, and are available as part of the `master AMR
metadata
spreadsheet <ftp://ftp.patricbrc.org/BRC_Mirrors/AMR/PATRIC_genomes_AMR.xlsx>`__
on the FTP site.

We have added additional project descriptions and experimental data from
two of the NIAID Functional Genomics Centers: The Chicago Center for
Functional Annotation (CCFA) and Genes Unknown in *Acinetobacter
baumannii* (GUNK). These are available from the respective pages in
PATRIC:
`CCFA <http://enews.patricbrc.org/the-chicago-center-for-functional-annotation-ccfa/>`__
and
`GUNK <http://enews.patricbrc.org/genes-unknown-in-acinetobacter-baumannii-gunk/>`__. 
We have also added project descriptions and data from the Omics4TB
Disease Progression, a NIAID Systems Biology Center, available from the
`Omics4TB <http://enews.patricbrc.org/omics4tb/>`__ page in PATRIC.
