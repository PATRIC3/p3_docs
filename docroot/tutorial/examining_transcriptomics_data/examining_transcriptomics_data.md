# Examining Transcriptomics Data

## I. Finding Experimental Data available in PATRIC
1. PATRIC has imported experimental data from several prominent genera, most notably Escherichia and Mycobacterium.  To find this data, click on a genus of interest on the Organisms tab (or use the global search) and select a genus of interest.

    ![Step 1](./images/image1.png "Step 1")

2. This will take you to the landing page for that genus.  To see if any transcriptomic data is available, click on the Transcriptomics tab (red arrow).

    ![Step 2](./images/image2.png "Step 2")

3. This will open a new page that shows all the experimental data available for that genus.
![Step 3](./images/image3.png "Step 3")

## II.  Finding Specific Experiments to Examine
1. PATRIC provides filter to help find specific experimental data.  To find that, click on the Filters icon, which is located on the far right side of the page (red arrow).
![Step 4](./images/image4.png "Step 4")

2. This will open up a filter that is on top of the table.  It allows researchers to filter on the experimental conditions, the type of mutant, the species, the strain, and if the experiment is a time series or not.
![Step 5](./images/image5.png "Step 5")

3. Clicking on any of the text in the filter will highlight it (red arrow).
![Step 6](./images/image6.png "Step 6")

4. This will re-filter the table to show all the experiments that have that particular tag.
![Step 7](./images/image7.png "Step 7")

## III. Examining a single experiment-Experiment filter
1. Clicking on the check box in front of the name of an experiment will highlight it (red arrow) and will also give information about the selected experiment in the area beyond the vertical green bar.
![Step 8](./images/image8.png "Step 8")

2. Once an experiment is selected, the green bar becomes populated with downstream processes that you can do with that selection.  In this case it includes downloading the information about the selection, creating a group that includes the selection, see the genes in that particular experiment, and viewing the experiment.  Click on the Genes icon.
![Step 9](./images/image9.png "Step 9")

3. This opens a new tab that shows all the genes and conditions from that particular experiment.
![Step 10](./images/image10.png "Step 10")

## IV. Examining genes within an experiment: Gene filter
1. A filter on the right side of the gene table where the genes in each experimental condition can be filtered on up- or down-regulation.  Clicking on one of the check boxes in front of a single experiment will re-filter the tables to meet that selection.

    ![Step 11](./images/image11.png "Step 11")

2. Clicking on a checkbox above this list of experimental conditions will auto-select all the conditions together, re-filtering the table to show all the genes that are similarly expressed across all conditions.
![Step 12](./images/image12.png "Step 12")

3. Many of the experiments examined more than one genome.  The filter table also provides the means to select specific genomes used within the experiment.  To do this, researchers need to click on the down arrow under Filter by Genome.  This will show all the genomes used in the experiment.  Clicking on one will re-filter the table to show only the results for that genome.

    ![Step 13](./images/image13.png "Step 13")

4. A text box provides the ability to search for the names of specific genes.  Entering text in that box and clicking on the Filter button will re-sort the table to show the genes that contained that word(s) in their functional description.
![Step 14](./images/image14.png "Step 14")

5. Researchers can also filter on the level of expression of specific genes by selecting a log ratio or Z score, and then clicking on the Filter button.  This will re-sort the table to show the number of genes that match that level of expression.

    ![Step 15](./images/image15.png "Step 15")

## V. Visualizing the genes and their expression on a heatmap
1. PATRIC also provides a way to visualize gene expression with a heatmap. Click on the Heatmap tab above the filter.

    ![Step 16](./images/image16.png "Step 16")

2. This will open a page that shows all the conditions and gene expression levels that match the selections made on the filter.

    ![Step 17](./images/image17.png "Step 17")

4.  Several buttons on the upper right above the heatmap allow researchers to flip the axis, putting experimental conditions on the x-axis and the genes on the y-axis.  The colors used in the heatmap can be changed. The genes can be clustered, which at the default Pearson correlation with pairwise average-linkage as the clustering type.  There is also an advanced clustering method, and a way to see the significant genes, or all the genes in the genome.

    ![Step 18](./images/image18.png "Step 18")

5. Clicking on advanced clustering open a pop-up window that allows researchers to cluster by genes, comparisons, or both.  In addition, there are several clustering algorithms and clustering types to choose from.

    ![Step 19](./images/image19.png "Step 19")

6. Clicking on any of the clustering algorithms will re-sort the heat map to group genes that are expressed similarly together across the conditions.

    ![Step 20](./images/image20.png "Step 20")

## VI. Getting the data about the genes from the heatmap visualization
1. To find further information on a group of genes in the heatmap, researchers can use their mouse to draw a box around genes, or patterns, of interest.

    ![Step 21](./images/image21.png "Step 21")

2. This action will generate a pop-up window that provides several options for viewing the data, including download the genes, showing them, adding them to a group, or downloading the heatmap data.

    ![Step 22](./images/image22.png "Step 22")

3. Clicking on Show Genes will open a new tab that shows the list of genes from the selection. Clicking on the check box next to Genome Name at the top of the table head will auto-select all the genes that where selected in the heatmap.
![Step 23](./images/image23.png "Step 23")

4. Once any, or all the genes are selected, a list of downstream analysis tools will appear in the vertical green bar.

    ![Step 24](./images/image24.png "Step 24")

5. These downstream tools or processes include the ability to download all the features in the table, go to the feature list view (Features icon), go to a view showing all the genomes that are the genes from the original selection belong to (Genomes icon), get the amino acid or nucleotide fasta files for all genes selected (FASTA icon), generate a multiple sequence alignment (MSA icon), map the PATRIC genes to other identifiers like UniProt (ID Map icon), find out any pathways that the selected genes belong to (Pathway icon), or to add the genes to an existing group, or create a new group with the selected genes (Group icon).

    ![Step 25](./images/image25.png "Step 25")

6. If the Pathway Summary icon is selected, a new tab will open with a table showing this information.  This may take some time, depending on the number of genes selected.  A page with a spinning wheel will be displayed while PATRIC recovers the information.

    ![Step 26](./images/image26.png "Step 26")

7. Once the table loads, a list of the pathways, the number of genes from the original selection, the number of genes in the genome that are part of the pathway, and the percent coverage (the selected genes as opposed to the total genes in the genome that are part of the pathway) are displayed.

    ![Step 27](./images/image27.png "Step 27")

8. Clicking on an individual pathway open a list of downstream processes in the vertical green bar.
![Step 28](./images/image28.png "Step 28")

9. Clicking on the pathway map icon will open a new page that shows a list of genes based on their EC number on the left, and a KEGG pathway map with the genes from that genome displayed on the right.  Clicking on the legend at the top right of the page shows the genes with those specific EC numbers that are annotated in the genome (green box).  The genes that were part of the original selection from the heatmap will be colored blue.
![Step 29](./images/image29.png "Step 29")

## VII. Examining multiple experiments
1. Researchers can compare more than one experiment for the same organism by clicking on the experiment titles in front of the name.
![Step 30](./images/image30.png "Step 30")

2. This may take some time, so the spinning wheel will show that PATRIC is working to display the data selected.
![Step 31](./images/image31.png "Step 31")

3. This opens a new tab that shows all the genes and conditions from that selected experiments.
![Step 32](./images/image32.png "Step 32")

4. The same ability of filtering by up- or down-regulation, genome name, or log-ratio/Z-score can be deployed by making a selection and clicking on the Filter button.

    ![Step 33](./images/image33.png "Step 33")

5. The heatmap view shows the results of the filtering on the various experiments selected.  Clicking on the Cluster icon will cluster the results across all experiments and conditions.
![Step 34](./images/image34.png "Step 34")

6. The information on specific genes can be viewed by using the mouse to draw a box over the selection, as described above.

    ![Step 35](./images/image35.png "Step 35")

## VIII.  Expression at the Gene level - Transcriptomics
1. Genes can be found by global search, or by selecting a specific gene from a table (red arrow). This populates the vertical green band with possible downstream functions. Clicking on the Feature icon (blue arrow) will open a new tab that is the landing page for the Feature page.  
![Step 36](./images/image36.png "Step 36")

2. Once on the gene landing page, clicking on the Transcriptomics tab will show if there is any available expression data for the gene in PATRIC.
![Step 37](./images/image37.png "Step 37")

3. If data is available, the Transcriptomics tab will show first two charts that show the levels of expression based on Log ratio or Z score based on all the available data. A pie chart showing the strains, gene modification, or experimental conditions is also presented.
![Step 38](./images/image38.png "Step 38")

4. Inserting text in the filter (red arrow) and clicking on the filter button will filter the conditions, showing the expression levels based on the experimental conditions that meet the search criteria. Filtering on the Log ration (blue arrow) or Z score will also filter the results.
![Step 39](./images/image39.png "Step 39")

5. Clicking on the Table (red arrow) will rewrite the table to show a list of the conditions that the gene is expressed in.
![Step 40](./images/image40.png "Step 40")

6. Clicking on a specific condition (red arrow) wills how the information about that condition in the box beyond the vertical green band. It will also populate the vertical green band with downstream processes that apply.
![Step 41](./images/image41.png "Step 41")

## IX.  Expression at the Gene level – Correlated Genes
1. Clicking on the Correlated Genes tab (red arrow) will show the genes that are either up or down-regulated with the gene on the Feature page. The numbers are based on the public transcriptomics data that are available in PATRIC.
![Step 42](./images/image42.png "Step 42")

2. Researchers can filter the correlated genes based on positive or negative correlation
![Step 43](./images/image43.png "Step 43")

3. Results can also be filtered on the correlation cutoff level.
![Step 44](./images/image44.png "Step 44")
