:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/tutorial/taxonomic_classification/taxonomic_classification.rst

===================================
Taxonomic Classification at PATRIC
===================================

Metagenomics is the study of genomic sequences obtained directly from an
environment. For many metagenomic samples, the species, genera and even
phyla present in the sample are largely unknown at the time of
sequencing, and the goal of sequencing is to determine the microbial
composition as precisely as possible. The PATRIC Taxonomic
Classification service can be used to identify the microbial composition
of metagenomic samples. Researchers can submit their metagenomic samples
that are reads (paired-or single-end, long or short, zipped or not) to
the service, as well as, Sequence Read Archive accession numbers or
contigs.

**I. Locating the Taxonomic Classification Service App.**

   1. At the top of any PATRIC page, find the Services tab.

   |image0|

   2. Click on Taxonomic Classification.

   |image1|

   3. This will open up the Taxonomic Classification landing page where
   researchers can submit long reads, single or paired read files, an
   SRA run accession number, or assembled contigs to the service.

   |image2|

**II. Uploading paired end reads.** Many paired read libraries are given
as file pairs, with each file containing half of each read pair. Paired
read files are expected to be sorted in such a way that each read in a
pair occurs in the same Nth position as its mate in their respective
files. These files are specified as READ FILE 1 and READ FILE 2. For a
given file pair, the selection of which file is READ 1 and which is READ
2 does not matter.

   1. To upload a fastq file that contains paired reads, locate the box
   called “Paired read library.”

   |image3|

   2. The reads must be located in the workspace. To initiate the
   upload, first click on the folder icon.

   |image4|

   3. This opens up a window where the files for upload can be selected.
   Click on the icon with the arrow pointing up.

   |image5|

   4. This opens a new window where the file you want to upload can be
   selected. Click on the “Select File” in the blue bar.

   |image6|

   5. This will open a window that allows you to choose files that are
   stored on your computer. Select the file where you stored the fastq
   file on your computer (red arrow) and click “Open”.

   |image7|

   6. Once selected, it will autofill the name of the file. You can see
   it in the screenshot below. Click on the Start Upload button.

   |image8|

5. This will auto-fill the name of the document into the text box as
seen below.

   |image9|

   6. Pay attention to the upload monitor in the lower right corner of
   the PATRIC page. It will show the progress of the upload. Do not
   submit the job until the upload is 100% complete.

   |image10|

   7. Repeat steps 2-5 to upload the second pair of reads.

   |image11|

   8. To finish the upload, click on the icon of an arrow within a
   circle. This will move your file into the Selected libraries box
   |image12|

**III. Uploading single reads**

   1. To upload a fastq file that contains single reads, locate the text
   box called “Single read library.”

   |image13|

   2. If the reads have previously been uploaded, click the down arrow
   next to the text box below Read File.

   |image14|

   3. This opens up a drop-down box that shows the all the reads that
   have been previously uploaded into the user account. Click on the
   name of the reads of interest.

   |image15|

   4. This will auto-fill the name of the document into the text box as
   seen below.

   |image16|

   5. To finish the upload, click on the icon of an arrow within a
   circle. This will move your file into the Selected libraries box
   where it is ready to be assembled

   |image17|

**IV. Submitting reads that are present at the Sequence Read Archive
(SRA)**

1. PATRIC also supports analysis of existing datasets from SRA. To
   submit this type of data, locate the Run Accession number and copy
   it.

..

   |image18|

2. Paste the copied accession number in the text box underneath SRA Run
   Accession, then click on the icon of an arrow within a circle.

..

   |image19|

3. This will move the file into the Selected libraries box where it is
   ready to be assembled

..

   |image20|

**V. Submitting assembled contigs**

   1. To submit a taxonomic classification job that uses contigs, click
   on the check box in front of Assembled Contigs in the upper box.
   Clicking on the folder icon.

   |image21|

   2. This will open a pop-up window that shows data in the private
   workspace that can be selected. The upload icon in the upper right
   can also be used to upload contig files that might exist on your
   computer.

   |image22|

3. Clicking on the down arrow next to the contigs text box will show .fa
   files that have been recently accessed in the private workspace.

   |image23|

**VI. Selecting parameters.**

   1. Parameters must be selected prior to job submission. The algorithm
   used for Taxonomic Classification is Kraken2[1], which uses exact
   alignment of k-mers for classification accuracy. The Kraken2
   algorithm was downloaded from the following source:
   https://ccb.jhu.edu/software/kraken2/

   |image24|

   2. Click on the down arrow at the end of the text box under Database
   to see the possible selections. All genomes is the standard Kraken 2
   database[1] (generated 23 October 2018) containing distinct 31-mers,
   based on completed microbial genomes from NCBI. RDP is the Ribosomal
   Database Project (RDP)[2], a curated database that offers
   ribosome-related data that draws on data from major sequence
   repositories. SILVA is a ribosomal RNA gene database that contains
   aligned ribosomal RNA (rRNA) gene sequences from the Bacteria,
   Archaea and Eukaryota domains[3]. Clicking on a database will change
   the default selection of All genomes.

   |image25|

4. Sequences that map to identified taxa, as well as those that don’t
   map to anything, can be saved and will be available in the output
   folder when the job is completed.

   |image26|

5. A folder must be selected for the Taxonomic Classification job.
   Clicking on the down arrow at the end of the text box underneath
   Output Folder will show recent folders that have been used. Clicking
   on the folder icon at the end of the text box will open a pop-up
   window where all folders can be viewed, or new folders created.

   |image27|

6. A name for the job must be entered in the text box under Output Name.
   At this point, the Submit button turns blue and the job will be
   submitted once clicked.

   |image28|

7. A successful submission will generate a message indicating that the
   job has been queued.

..

   |image29|

   7. The bottom of each PATRIC page has an indicator that shows the
   number of jobs that are queued, running or completed. Clicking on the
   word Jobs will rewrite the page to show the Job status.

   |image30|

**VI. Viewing the Taxonomic Classification job.**

1. Researchers must monitor the Jobs Status page to see the status of
   their job, which is indicated in the first column (Queued, Running,
   Complete, Failed).

   |image31|

2. Clicking on the row that contains the job of interest will open two
   icons in the vertical green bar. If there is a problem with a
   particular job, the Report Issue icon should be clicked.

   |image32|

3. This will open a pop-up window where issues with particular jobs can
   be reported. A description of the particular problem can be provided,
   and clicking the submission button will generate a message to PATRIC
   team members, notifying them that there has been a problem. We
   encourage researchers to report all failed jobs, or those that have
   results that are confusing. In addition, researchers should report
   long waits that they are experiencing in the queue.

   |image33|

4. A job that has been successfully completed can be viewed by clicking
   on the row and then clicking on the View icon in the vertical green
   bar.

   |image34|

5. This will open page for the selected job. The top box has the job ID
   number and gives pertinent information about the time it took to
   complete and the selected parameters. The lower table has five output
   files.

..

   |image35|

6. Click on the TaxonomicReport.html. This will populate the vertical
   green bar with a number of icons. Clicking the information icon (i)
   will open a new tab that has the Taxonomic classification tutorial.
   There are icons for downloading the data, viewing it, deleting the
   file, renaming the file, copying or sharing with another PATRIC user,
   moving it to a different director, or changing the type tagged to the
   file. To examine the TaxonomicReport.html, click on the View
   icon.\ |image36|

7. This page shows Kraken 2's standard sample report format, which is
   tab-delimited with one line per taxon. The fields of the output, from
   left-to-right, are as follows:

   1. Percentage of fragments covered by the clade rooted at this taxon

   2. Number of fragments covered by the clade rooted at this taxon

   3. Number of fragments assigned directly to this taxon

   4. A rank code, indicating (U)nclassified, (R)oot, (D)omain,
   (K)ingdom,

   (P)hylum, (C)lass, (O)rder, (F)amily, (G)enus, or (S)pecies.

   Taxa that are not at any of these 10 ranks have a rank code that is

   formed by using the rank code of the closest ancestor rank with

   a number indicating the distance from that rank. E.g., "G2" is a

   rank code indicating a taxon is between genus and species and the

   grandparent taxon is at the genus rank.

   5. NCBI taxonomic ID number

   6. Indented scientific name

..

   |image37|

8. Clicking on any of the names in the blue text will open the landing
   page for the selected taxon.

..

   |image38|

9.  To see an interactive, visual description of the results select the
    chart.html from the job page and click the View icon.

    |image39|

10. This will open a pie chart view of the results which gives a visual
    representation of the reads mapping to each taxon. |image40|

11. The chart view is interactive. Clicking on a taxon within the pie
    chart will provide a summary of the reads mapping to that specific
    selection on the upper right corner.

    |image41|

12. The complete data can be found in the report.txt, which is a
    downloadable (or viewable) text document summarizing the results.

    |image42|

13. The full_report.txt is a downloadable text file of the results seen
    in the report.txt file, but also includes taxonomy entries for which
    there were zero hits.

    |image43|

14. The output.txt.gz contains information about each input sequence.
    This will be a large file that should be downloaded in order to view
    it.

..

   |image44|

**References**

1. Wood, D.E. and S.L. Salzberg, *Kraken: ultrafast metagenomic sequence
classification using exact alignments.* Genome biology, 2014.
**15**\ (3): p. R46.2. Maidak, B.L., et al., *The RDP (ribosomal
database project) continues.* Nucleic acids research, 2000. **28**\ (1):
p. 173-174.3. Quast, C., et al., *The SILVA ribosomal RNA gene database
project: improved data processing and web-based tools.* Nucleic acids
research, 2012. **41**\ (D1): p. D590-D596.

.. |image0| image:: media/image1.emf
   :width: 5.47222in
   :height: 0.54607in
.. |image1| image:: media/image2.png
   :width: 5.62222in
   :height: 1.84104in
.. |image2| image:: media/image3.png
   :width: 5.11111in
   :height: 5.51793in
.. |image3| image:: media/image4.png
   :width: 4.40278in
   :height: 3.15278in
.. |image4| image:: media/image5.png
   :width: 6.5in
   :height: 2.41875in
.. |image5| image:: media/image6.png
   :width: 5.34722in
   :height: 1.70357in
.. |image6| image:: media/image7.png
   :width: 6.09722in
   :height: 3.86418in
.. |image7| image:: media/image8.png
   :width: 6.5in
   :height: 2.79722in
.. |image8| image:: media/image9.png
   :width: 6.5in
   :height: 4.27014in
.. |image9| image:: media/image10.png
   :width: 5.43056in
   :height: 1.88889in
.. |image10| image:: media/image11.png
   :width: 5.63889in
   :height: 1.58142in
.. |image11| image:: media/image12.png
   :width: 5.63889in
   :height: 2.0694in
.. |image12| image:: media/image13.png
   :width: 5.36111in
   :height: 2.18053in
.. |image13| image:: media/image14.png
   :width: 2.93056in
   :height: 2.0714in
.. |image14| image:: media/image15.png
   :width: 2.65278in
   :height: 1.78932in
.. |image15| image:: media/image16.emf
   :width: 3.42in
   :height: 1.52in
.. |image16| image:: media/image17.png
   :width: 2.77778in
   :height: 1.88467in
.. |image17| image:: media/image18.png
   :width: 4.59722in
   :height: 1.62769in
.. |image18| image:: media/image19.png
   :width: 4.60926in
   :height: 3.40278in
.. |image19| image:: media/image20.png
   :width: 4.125in
   :height: 2.67708in
.. |image20| image:: media/image21.png
   :width: 5.75221in
   :height: 2.01389in
.. |image21| image:: media/image22.png
   :width: 4.36549in
   :height: 2.125in
.. |image22| image:: media/image23.png
   :width: 5.41917in
   :height: 3.76389in
.. |image23| image:: media/image24.png
   :width: 5.31969in
   :height: 2.88889in
.. |image24| image:: media/image25.png
   :width: 4.35409in
   :height: 3.54167in
.. |image25| image:: media/image26.png
   :width: 4.73611in
   :height: 3.86111in
.. |image26| image:: media/image27.png
   :width: 4.65in
   :height: 3.875in
.. |image27| image:: media/image28.png
   :width: 4.13889in
   :height: 3.37771in
.. |image28| image:: media/image29.png
   :width: 4.55556in
   :height: 3.56944in
.. |image29| image:: media/image30.png
   :width: 6.31641in
   :height: 0.68056in
.. |image30| image:: media/image31.png
   :width: 4.77102in
   :height: 1.70833in
.. |image31| image:: media/image32.png
   :width: 6.16406in
   :height: 2.77778in
.. |image32| image:: media/image33.png
   :width: 6.5in
   :height: 1.54514in
.. |image33| image:: media/image34.png
   :width: 5.64353in
   :height: 3.94444in
.. |image34| image:: media/image35.png
   :width: 6.5in
   :height: 1.28333in
.. |image35| image:: media/image36.png
   :width: 6.37954in
   :height: 2.61111in
.. |image36| image:: media/image37.png
   :width: 6.18326in
   :height: 2.83333in
.. |image37| image:: media/image38.png
   :width: 5.47285in
   :height: 2.875in
.. |image38| image:: media/image39.png
   :width: 6.00093in
   :height: 4.125in
.. |image39| image:: media/image40.png
   :width: 6.15446in
   :height: 2.48611in
.. |image40| image:: media/image41.png
   :width: 5.66667in
   :height: 2.74918in
.. |image41| image:: media/image42.png
   :width: 5.86787in
   :height: 3.05556in
.. |image42| image:: media/image43.png
   :width: 6.5in
   :height: 2.49861in
.. |image43| image:: media/image44.png
   :width: 6.5in
   :height: 2.53472in
.. |image44| image:: media/image45.png
   :width: 6.5in
   :height: 2.29028in
