:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/20170731-patric-july-2017-release.rst

PATRIC July 2017 Data and Website Release
=========================================

.. feed-entry::
   :date: 2017-07-31

PATRIC July 2017 Release Features over 3900 New Genomes, and New Functionality and Data Including a New Phylogenetic Tree Building Service and Enhancements to Multiple Services and Tools.

.. cut::

Data Updates:
--------------

New Genomes

In this release, PATRIC has added 3902 new genomes and associated metadata, bringing the total number of genomes in PATRIC to over 108,000. The full list of available bacterial genomes can be accessed from the Genomes Tab for all bacteria, and from the Genomes Data Landing Page.

Enhanced AMR landing pages


The updated Antimicrobial Resistance (AMR) landing page in PATRIC provides consolidated information and examples of data in PATRIC relevant to AMR including summaries for antibiotic information, AMR phenotypes, AMR genes, and AMR regions.  The AMR Landing Page in PATRIC is available from the Data Menu in the PATRIC menu bar and directly from https://www.patricbrc.org/view/DataType/AntibioticResistance.

Host Response Data Sets and API


PATRIC now includes 22 host-response expression data sets, including 2 from the NIAID-funded Omics4TB Systems Biology Center. The host response data sets are available from the Transcriptomics tab of the Homo sapiens genome view (https://www.patricbrc.org/view/Genome/9606.33#view_tab=transcriptomics) and the Transcriptomics tab of the Mus musculus genome view (https://www.patricbrc.org/view/Genome/10090.24#view_tab=transcriptomics). All host-response datasets are accessible via a newly developed host-response data API as part of inter-BRC pilot project.

New Services:
--------------

Phylogenetic Tree Service

The new Phylogenetic Tree Service enables construction of custom phylogenetic trees for up to 50 user-selected genomes. The service builds trees using conserved protein sequences, which is the same methodology used to build the public genus-level phylogenetic trees in the PATRIC website. The Phylogenetic Tree Service is available from the Services Menu in the PATRIC menu bar and directly from https://www.patricbrc.org/app/PhylogeneticTree.

Host ID-Mapping Service

The new Host-ID Mapping Service allows mapping of gene expression data using multiple identifier schemes, e.g. RefSeq locus tags, transcript/protein IDs, Ensembl gene IDs, etc. The Host ID-Mapping Service is available through the PATRIC Command Line Interface (CLI), available from the PATRIC3 GitHub site.

Enhanced Services and Tools:
----------------------------

Nucleotide MSA and Tree Viewer

The coupled MSA and Tree Viewer has been updated to support nucleotide sequence gene alignments.  Users can now also filter alignment based on percent conservation or gaps to identify SNPs and indels. The updated viewer is accessible by clicking the MSA icon on the green “Action Bar” after selecting a set of nucleotide sequences.

Host Differential Expression Data Support

The PATRIC Expression Import Service now supports eukaryotic host differential expression data.   The data can be associated with the host reference genomes in PATRIC, including human, rhesus macaque, pig, mouse, rat, ferret, chicken, zebrafish, fruit fly, and roundworm. The Expression Import Service is available from the Services Menu in the PATRIC menu bar and directly from https://www.patricbrc.org/app/Expression.

Tn-seq Alignment Files in Genome Browser

Users can now view the alignment results of the Tn-seq Analysis Service to the reference genome in the Genome Browser. The alignments are presented as a separate track in the Genome Browser along with annotated genes.  The Tn-seq Analysis Service is available from the Services Menu in the PATRIC menu bar and directly from https://www.patricbrc.org/app/Tnseq.

New AMR classifiers

The PATRIC Genome Annotation Service now includes AMR classifiers for Klebsiella pneumoniae. This is part of an ongoing effort to incorporate AMR-related annotations based on newly acquired or analyzed data from AMR studies.  The Genome Annotation Service is available from the Services Menu in the PATRIC menu bar and directly from https://www.patricbrc.org/app/Annotation.

Global Search Enhancements

The PATRIC Global Search now provides more user-friendly means to search for all or any search terms provided, with exact or partial matches. This is helpful while searching for list of genomes/genes in a single query, or searching for particular identifiers. The Global Search is available at the top-left of the PATRIC website.

Workspace Enhancements:
-----------------------
Workspace Data Management

New features in the Private Workspace allow users to create multiple workspaces, share them with other users, and/or make them public. Users can also now edit, copy, move, and delete workspace content. The Private Workspace is available from the Workspaces Menu (“home” option) after logging in.

Genome metadata submission / editing for user genomes

Users can now edit the metadata associated with their private genomes including information regarding isolation location, host, phenotype, and dozens of other metadata fields.

Generic Workspace Object Viewer

This feature facilitates viewing of text, HTML and image files in the workspace directly in the browser, without the need to download the file and open in a separate application.
