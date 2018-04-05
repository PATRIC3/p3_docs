# Correlated Genes Tab

## Overview
The Correlated Genes Tab shows the genes that are either up or down-regulated with respect to selected gene in the Feature View. The values are based on the public transcriptomics data that are available in PATRIC. 

### See also
  * [Examining Transcriptomics Data Tutorial](https://docs.patricbrc.org//tutorial/examining_transcriptomics_data/examining_transcriptomics_data.html)
  * [Transcriptomics Gene List](../organisms_taxon/transcriptomics_gene_list.html)
  * [Transcriptomics Gene List Heatmap](../organisms_taxon/transcriptomics_gene_heatmap.html)
  * [Transcriptomcs Tab, Gene-Level](../organisms_gene/transcriptomics.html)
  * [Expression Data Import Service](../services/expression_data_import_service.html)

Most of the PATRIC transcriptomics data have been curated from published gene expression datasets related to bacterial pathogens in [NCBI's GEO database](http://www.ncbi.nlm.nih.gov/geo/). Some additional data sets have been incorporated from the NIAID-funded [Systems Biology](https://patricbrc.org/webpage/website/data_collections/niaid_systems_biology.html) and [Functional Genomics](https://patricbrc.org/webpage/website/data_collections/niaid_functional_genomics.html) Centers and other sources.

## Accessing the Correleated Genes on the  PATRIC Website
Clicking the Correlated Genes tab in the Feature View displays a table showing all the genes with expression data in PATRIC that are either up or down-regulated with respect to selected gene. 

![Correlated Genes Table](../images/transcriptomics_correlated_genes.png)


 
### Correlated Genes Table Tools
You may do the following with the table:

* **Download** the entire contents of the data used to create the charts in text, CSV, or Excel format by clicking the Download button above the table on the left side.

* **Filter** the included expression levels based on the experimental conditions that meet the search criteria entered in the Keyword text box. Filtering on the Log ratio or Z score will also filter the results to the specified cut-off score. Clicking the Filter button sets the filter, clicking the Reset Filter sets the charts back to the original display with all values.

The columns in the table include the following: 

* **Title:** The title of the transcriptomics experiment
* **PubMed:** The PubMed ID of the experiment
* **Accession:** The accession number (typically GEO) of the experiment
* **Strain:** The strain name of the genome
* **Gene Modification:** Modification of the gene, if any
* **Experimental Condition:** The experimental condition
* **Time Point:** Time point during the experiment, if time course
* **Avg Intensity:** 
* **Log Ratio:** Log ratio value of the expression level based on all available data
* **Z-score:** Z-score of the expression level based on all available data
 
### Action buttons

After selecting one or more of the experiments by clicking the checkbox beside the Title column in the table, a set of options becomes available in the vertical green Action Bar on the right side of the table.  These include

* **Hide/Show:** Toggles (hides) the right-hand side Details Pane.
* **Download:**  Downloads the selected items (rows).
* **Copy:** Copies the selected items to the clipboard.
