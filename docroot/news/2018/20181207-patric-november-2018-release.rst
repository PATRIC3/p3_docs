:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/2018/20181207-patric-november-2018-release.rst

PATRIC November 2018 Data and Website Release
==============================================

.. feed-entry::
   :date: 2018-12-07

This PATRIC release includes a new Genome Comparison Service; enhancements to the Metagenomic Binning, Tn-Seq, and RNA-Seq Services; 5 new instructional videos; and over 10,000 new microbial genomes.  

.. cut::


Data Updates:
--------------

**New Genomes**

In this release, PATRIC has added over 10,000 new genomes and associated metadata, bringing the total number of genomes and plasmids to over 200,000. The full list of available microbial and host genomes can be accessed `here
<https://www.patricbrc.org/view/GenomeList/?or(keyword(Bacteria),keyword(Archaea),keyword(Eukaryota))#view_tab=genomes>`__.


New Website Features:
----------------------

**Genome Comparison Service** This new service (Beta version) implements wraps progressiveMauve to produce and a whole genome alignment of two or more genomes. The resulting alignment can be visualized within the PATRIC website, providing insight into homologous regions and changes due to DNA recombination. The `Genome Comparison Service <https://patricbrc.org/app/GenomeAlignment>`_ is available from the Services top menu.

The assembly component of the **Metagenomic Binning Service** has been migrated to a 1024-node cluster, enabling a 10-fold increase in the throughput of assembly-based binning jobs. The `Metagenomic Binning Service <https://patricbrc.org/app/MetagenomeBinning>`_ is available from the Services top menu.

The **RNA-Seq Analysis Service** now supports direct import of sequence data from SRA, alleviating the need to first download the data from SRA and then upload into the service. The `RNA-Seq Analysis Service <https://patricbrc.org/app/Rnaseq>`_ is available from the Services top menu. 


PATRIC now has bacteriophage genome data and related functionalty. Included are 4,722 phage genomes from GenBank, annotated using PATRIC’s phage-specific annotation service. Phage protein families have been constructed to support comparative analysis. The `Similar Genome Finder Service
<https://patricbrc.org/app/GenomeDistance>`_ can be used to identify similar genomes and phage genes and proteins cam be searched using the new phage-specific `BLAST
<https://patricbrc.org/app/BLAST>`_ databases.  All phages and related data are accessible from the PATRIC homepage, `here
<https://patricbrc.org/view/Taxonomy/10239>`_.  


Migrated the assembly component of the Metagenomic Binning analysis tool to take advantage of Bebop, a 1024-node cluster operated by the Laboratory Computing Resource Center at Argonne National Laboratory, enabling an order-of-magnitude increase in the throughput of assembly-based binning jobs

Enhancement to RNA-Seq Service to enable direct import of sequence data from SRA

Enhancement to the Tn-Seq Service to use the new version of the TRANSIT software from Tom Ioerger’s group (Omics4TB)

Five new short instructional videos demonstrating how to perform some common useful tasks in PATRIC



