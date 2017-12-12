:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/20171130-patric-november-2017-release.rst

PATRIC November 2017 Data and Website Release
==============================================

.. feed-entry::
   :date: 2017-11-30

The PATRIC November 2017 Release Features over 20,000 new genomes, as well as new functionality and data Including a
production release of the Command Line Interface (CLI), FTP-based bulk upload capability, enhancements to the
Phylogenetic Tree Building Service, updated Tutorials, and other enhancements.

.. cut::


Data Updates:
--------------

**New Genomes**

In this release, PATRIC has added over 20,000 new genomes and associated metadata, bringing the total number of genomes
in PATRIC to over 135,000. Included in the new genomes are over 3500 assembled from SRA with AMR panel data. The full
list of available bacterial genomes can be accessed from the `Genomes Tab for all bacteria
<https://www.patricbrc.org/view/Taxonomy/2>`__, and from the `Genomes Data Landing Page
<https://www.patricbrc.org/view/DataType/Genomes>`__.

New Features:
--------------
**Command Line Interface**

This release includes an updated, production-level version of the Command Line Interface (CLI) to PATRIC. New commands
and features added to the CLI include those to

* allow access to PATRIC workspaces
* run PATRIC services, including Genome Assembly and Annotation
* manage typed objects in the workspace, such as genomes
* facilitate data access and manipulation

The CLI release also includes documentation containing instructions and commands for

* user authentication
* composing individual commands into pipelines
* managing workspaces
* accessing data in the database
* working with genome-typed objects
* annotating new genomes with RASTtk
* performing comparative analyses between groups of genomes, features, and data objects

The CLI is available from the `PATRIC3 GitHub Site <https://github.com/PATRIC3/PATRIC-distribution/releases>`__.
Tutorials for using the CLI are available from the `PATRIC CLI Help Documentation
<https://docs.patricbrc.org/cli_tutorial/index.html>`__.

**Bulk Upload Via FTPS**

The November Release includes the capability for bulk upload, download, and file browsing of data via FTPS. This service
is available by using FTPS to workspace.patricbrc.org and is compatible with `FileZilla
<https://filezilla-project.org/>`__ and `LFTP <http://lftp.tech/>`__, for example.

Enhancements:
--------------

**Phylogenetic Tree Service**

The Phylogenetic Tree Building Service now can stream trees to the interactive PATRIC tree viewer, which enables
phylogram/cladogram view, re-orientation of the tree, collapsing/expanding of clades, links to the genomes in PATRIC,
and other features. The Phylogenetic Tree Service is available from the Services Menu in the PATRIC menu bar and
directly from https://www.patricbrc.org/app/PhylogeneticTree.