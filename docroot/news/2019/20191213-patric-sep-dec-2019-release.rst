:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/2019/20191213-patric-sep-dec-2019-release.rst

PATRIC Data and Website Releases, September – December 2019
===========================================================

.. feed-entry::
   :date: 2019-12-13

This PATRIC release includes a new Genome Assembly Service, new Heatmap Viewer, new analysis Job Scheduler, and over 24,500 new microbial genomes.  


.. cut::


Data Updates:
--------------

**New Genomes**

Over the past 3 months, PATRIC has added XXX new genomes bringing the total number of genomes and plasmids in PATRIC to over 290,000. This includes XXX microbial genomes and XXX phage genomes. Data releases by month were the following:

   * September: XXX microbial genomes, XXX phage genomes
   * October: 17,575 microbial genomes, 403 phage genomes
   * November: 9,807 microbial genomes, 53 phage genomes
   
The November release included new manually curated AMR phenotype data for 6,797 genomes, which was collected from 14 publications. The taxonomy, BLAST, and MinHash databases and PATRIC FTP site have been updated to reflect these new genomes. The full list of available microbial and host genomes can be accessed `here
<https://www.patricbrc.org/view/GenomeList/?or(keyword(Bacteria),keyword(Archaea),keyword(Eukaryota))#view_tab=genomes>`__.


New Website Features:
----------------------
We have released a new **Genome Assembly Service**. This service replaces the prior PATRIC Genome Assembly Service, providing updated and improved algorithms including SPAdes, Unicycler, and Canu, and new features including hybrid assembly (PacBio and Illumina) and polishing using Racon and Pilon. The `Genome Assembly Service <https://www.patricbrc.org/app/Assembly2>`_ is available from the Services top menu on the website. 

We also released a new interactive **heatmap viewer**.  This html5/WebGL-based viewer replaces the previous Flash-based viewer in PATRIC. This change was made to migrate off of Flash, which will soon no longer be supported.  It also improves performance and includes additional features, such as the ability to change the colors used and SVG-format download. The Heat Map Viewer is used to present data in the Protein Family Sorter, gene expression comparison, pathway comparison, and subsystem comparison pages in PATRIC.  Examples can be seen here and here.

Finally, we have replaced the backend **job scheduler**, which manages the execution of the PATRIC analysis services. We are now using the Slurm Workload Manager to handle the allocation of PATRIC jobs to our compute cluster. This change will allow us to more easily and reliably add resources to the cluster, and to ensure fair allocation of these resources to our users. PATRIC analysis services are available from the Services top menu on the website.
