:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/2020/20200331-patric-jan-mar-2020-release.rst

PATRIC Data and Website Releases, January – March 2020
===========================================================

.. feed-entry::
   :date: 2020-03-31

This PATRIC release includes a new Genome Assembly Service, new Heatmap Viewer, new analysis Job Scheduler, and over 31,000 new microbial genomes.  


.. cut::


Data Updates:
--------------

**New Genomes**

Over the past 3 months, PATRIC has added 31,523 new genomes bringing the total number of genomes and plasmids in PATRIC to over 293,000. This includes 26,443 microbial genomes and 5,080 phage genomes. Data releases by month were the following:

- September: 5,058 microbial genomes, 4,888 phage genomes
- October: 11,813 microbial genomes, 187 phage genomes
- November: 9,572 microbial genomes, 5 phage genomes
   
The November release included new manually curated AMR phenotype data for 6,797 genomes, which was collected from 14 publications. The taxonomy, BLAST, and MinHash databases and PATRIC FTP site have been updated to reflect these new genomes.  Click the links to access the full list of available `bacterial <https://patricbrc.org/view/Taxonomy/2#view_tab=genomes>`_, `archaeal <https://patricbrc.org/view/Taxonomy/2157>`_, and `phage <https://patricbrc.org/view/Taxonomy/10239>`_ genomes.

New Website Features:
----------------------
We have released a new **Genome Assembly Service**. This service replaces the prior PATRIC Genome Assembly Service, providing updated and improved algorithms including SPAdes, Unicycler, and Canu, and new features including hybrid assembly (PacBio and Illumina) and polishing using Racon and Pilon. The `Genome Assembly Service <https://www.patricbrc.org/app/Assembly2>`_ is available from the Services top menu on the website. 

We also released a new interactive **heatmap viewer**.  This html5/WebGL-based viewer replaces the previous Flash-based viewer in PATRIC. This change was made to migrate off of Flash, which will soon no longer be supported.  It also improves performance and includes additional features, such as the ability to change the colors used and SVG-format download. The Heat Map Viewer is used to present data in the Protein Family Sorter, gene expression comparison, pathway comparison, and subsystem comparison pages in PATRIC.  Below are the links showing examples of protein family sorter and transcriptomics gene list with the new heat map viewer (click the heatmap option on the upper left side of the page to see the heatmap display): 

- `Protein family sorter with 11 Brucella genomes <https://patricbrc.org/view/GenomeList/?in(genome_id,(224914.11,262698.4,520448.3,520461.7,204722.5,444178.3,520459.3,568815.3,483179.4,359391.4,520456.3))#view_tab=proteinFamilies>`_
- `Transcriptomics gene list for Mycobacterium tuberculosis under nitric oxide treatment <https://patricbrc.org/view/TranscriptomicsExperiment/?eq(eid,(233094))>`_

Finally, we have replaced the backend **job scheduler**, which manages the execution of the PATRIC analysis services. We are now using the Slurm Workload Manager to handle the allocation of PATRIC jobs to our compute cluster. This change will allow us to more easily and reliably add resources to the cluster, and to ensure fair allocation of these resources to our users. PATRIC analysis services are available from the Services top menu on the website.
