:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/2018/20180131-patric-march-2018-release.rst

PATRIC March 2018 Data and Website Release
==============================================

.. feed-entry::
   :date: 2018-03-31

In this release, PATRIC has new subsystems functionality with precomputed subsystems for all PATRIC genomes as well as protein family updates. It also includes additional genome metadata with AMR panel data and new datasets from NIAID-funded centers.   This release also enhancements to the Circular Genome Viewer and a new PATRIC homepage design for evaluation and review.

.. cut::


Data Updates:
--------------

**New Subsystems, Protein Families, Genome Metadata, and Other Data Sets**

In this release, PATRIC has added precomputed subsystems and protein family updates for all public genomes.  The subsystem data is available through custom user interface displays, described below. It also includes additional genome metadata, including AMR panel data, for 13 bioprojects from JCVI as well as additional AMR metadata collected from publications by PATRIC curators.  Additionally, two datasets (proteomics and TRP phenotype) from the Omics4TB Systems Biology Center and new PPI data sets from the FLUTE Functional Genomics Center have been added as well, accessible `here
<https://www.patricbrc.org/webpage/website/data_collections/content/omics4tb.html>`__ and 
`here
<https://www.patricbrc.org/webpage/website/data_collections/content/flute.html>`__, respectively.


New Website Features:
----------------------

**Subsystems Functionality**

This release includes new pages for showing subsystem data for single genome, taxon, and genome group levels.  Subsystems are curated sets of biologically related functional roles across a reference set of genomes, comprising units of expert knowledge about a single biological process like a whole metabolic pathway (Glycolysis), or a piece of a pathway (L-2-amino-adipate to lysine module), the subunits of a multi-unit enzyme (Urease) or the pieces of a structural unit like the ribosome. Subsystem data at the summary, subsystem, and gene level can be found on the Subsystem tab in any Taxon View, as shown `here
<https://www.patricbrc.org/view/Taxonomy/234#view_tab=subsystems>`__. Corresponding subsystems updates have been incorporated into the PATRIC Genome Annotation Service, available `here
<https://www.patricbrc.org/app/Annotation>`__.

**Evaluation Version of New PATRIC Homepage Design**
We are working on a new homepage design for the website to clarify, simplify, and streamline access to the ever increasing data and functionality of the PATRIC resource. We invite feedback from PATRIC users which we will use to refine the design before conversion of the website.  The evaluation version is available `here
<https://www.alpha.patricbrc.org/home-new>`__.

**Enhancements to the Circular Genome Viewer**
The PATRIC Circular Genome Viewer now has tracks for highlighting specialty genes such as AMR, VF, transporters, and drug targets.  The layout has also been improved for genomes with large numbers of contigs.  Similar improvements have been made in the circular Proteome Comparison Viewer.  The Circular Genome Viewer can be accessed by clicking the Circular Viewer tab in any Genome View, as shown `here
<https://www.patricbrc.org/view/Genome/83332.12#view_tab=circular>`__.

**Enhancements to RNA-Seq Analysis Service**
*Note: Released April 7, 2018.* The RNA-Seq pipeline at PATRIC has been updated to use HISAT2 to generate alignments for reads and now uses FastQC and SAMStat to generate quality reports for fastq files and alignment files respectively. This new functionality allows users to assess how much of their sample has been aligned and to investigate potential causes of poor performance. In addition the pipeline now automatically generates PATRIC's Differential Expression objects so that users can investigate which genes are significantly up or down regulated between conditions using the PATRIC heatmap functionality. The RNA-Seq Analysis Service can be accessed `here
<https://patricbrc.org/app/Rnaseq>`__.






