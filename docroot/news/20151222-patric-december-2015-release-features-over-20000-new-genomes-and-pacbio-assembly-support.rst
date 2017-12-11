=========================================================================================
PATRIC December 2015 Release Features over 20,000 New Genomes and PacBio Assembly Support
=========================================================================================


:Date:   2015-12-22T16:03:53+00:00

**New Genomes and Annotation System Enhancements**

In this release, we have added 23,052 new genomes from NCBI GenBank,
bringing the total number of genomes in PATRIC to over 54,000. The full
list of available bacterial genomes can be accessed from the `Genomes
Tab for all
bacteria <https://www.patricbrc.org/portal/portal/patric/GenomeList?cType=taxon&cId=2&dataSource=&displayMode=&pk=&kw=>`__,
and from the `Genomes Data Landing
Page <https://www.patricbrc.org/portal/portal/patric/Genomes>`__.

As part of this Data Release, we have implemented an enhanced annotation
system and process that allows us to annotate and release new genomes
continuously—in a near real-time mode.  With this enhancement, we will
be able to maintain currency with other public genome sources such as
NCBI, as well as quickly incorporate new genomes from other sources.

Other recent enhancements to the annotation system include support for
the following key features:

-  Public/private flag for any genome submission
-  Efficient submission of large batch of genomes
-  Submission of GenBank files
-  Parsing of minimum metadata, i.e., genome name, taxon id, genetic
   code, directly from GenBank files
-  Parsing features from original GenBank files and preserving them as
   ID synonyms
-  Carrying forward additional “misc” features such as repeats, binding
   sites, miscellaneous RNAs, etc. annotated in the GenBank file to
   PATRIC annotations
-  Assigning functions based on the latest build of k-mers from
   Core-SEED
-  Assigning new protein families—PLFams and PGfams
-  Computation of MLSTs
-  Automated parsing of genome metadata from NCBI BioProject and
   BioSample records
-  Automated parsing of antibiogram metadata from NCBI BioSample records
-  Loading antibiogram metadata into the corresponding new PATRIC Solr
   database core
-  Automated incorporation of strain name into genome name, if not
   already present
-  Automated incrementing of genome counts for corresponding taxonomy
   nodes (for public genomes)

**Assembly Service Enhancements**

Also in this release, we have enabled experimental support for assembly
of genomes sequenced using PacBio technology and Oxford Nanopore
technologies. PATRIC users can now take advantage of the long reads
generated on these platforms and assemble them into longer contigs, and
in some cases complete genomes. Both raw bax.h5 read files and filtered
FASTQ files from PacBio and FASTQ from Oxford Nanopore are accepted as
input. The PATRIC Genome Assembly Service can be accessed at
https://www.patricbrc.org/app/Assembly. NOTE: You must have a PATRIC
user account and be logged in to use the services and workspace.
