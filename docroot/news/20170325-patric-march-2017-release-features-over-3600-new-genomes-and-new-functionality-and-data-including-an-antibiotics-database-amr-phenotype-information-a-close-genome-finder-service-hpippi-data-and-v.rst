:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/20170325-patric-march-2017-release-features-over-3600-new-genomes-and-new-functionality-and-data-including-an-antibiotics-database-amr-phenotype-information-a-close-genome-finder-service-hpippi-data-and-v.rst

==============================================================================================================================================================================================================================================================================================
PATRIC March 2017 Release Features over 3600 New Genomes, and New Functionality and Data Including an Antibiotics Database, AMR Phenotype Information, a Close Genome Finder Service, HPI/PPI Data and Visualization, a Compare Region Viewer, an ID-Mapping Tool, and Enhanced Global Search.
==============================================================================================================================================================================================================================================================================================

.. feed-entry::
   :date: 2017-03-25

**PATRIC March 2017 Data and Website Release: **



**New Genomes**

In this release, PATRIC has added 3669 new genomes, bringing the total
number of genomes in PATRIC to nearly 98,000. The full list of available
bacterial genomes can be accessed from the `Genomes Tab for all
bacteria <https://www.patricbrc.org/view/Taxonomy/2>`__, and from the
`Genomes Data Landing
Page <https://www.patricbrc.org/view/DataType/Genomes>`__. UniProt ID
Mappings have also been updated.

**Antibiotics Database**

PATRIC now has an antibiotics database that includes information such as
name, description, chemical structure, mechanism of action, and
pharmacology. Information is incorporated from PubChem for approximately
100 antibiotics for which PATRIC has AMR phenotype data. Antibiotics
data are displayed via a new Antibiotics Overview Page with tabs for:

-  Basic information / overview of the antibiotic and publications
   related to resistance to that antibiotic
-  All AMR phenotype data for a given antibiotic
-  Related AMR genes
-  Related AMR k-mer regions predicted by the classifiers

An example overview page for Amikacin can be accessed at
https://www.patricbrc.org/view/Antibiotic/?eq(antibiotic_name,amikacin)#view_tab=overview

**AMR Phenotype Data**

PATRIC has a new “AMR phenotypes” tab at the taxon and genome levels
that provides list of genomes, their AMR phenotypes, and corresponding
metadata about the laboratory methods and testing standards. The table
allows filtering by antibiotic and phenotype to create genome groups
containing resistant and susceptible genomes for that antibiotic. An
example can be accessed from
https://www.patricbrc.org/view/Taxonomy/1763#view_tab=amr&filter=and(eq(antibiotic,Amikacin),eq(resistant_phenotype,Susceptible))

Predicted AMR phenotypes from classifiers are now displayed on the
genome overview pages, including private user genomes annotated using
the PATRIC Annotation Service.

**Similar Genome Finder Service**

PATRIC now has a new Close Genome Finder Service that, for a
user-selected public or private genome, or for an uploaded FASTA file,
will find the closest related public genomes (by sequence) in PATRIC
using the MInHash algorithm to perform comparisons. The service is
available from the Services menu at
https://www.patricbrc.org/app/GenomeDistance.

**Host-Pathogen Interaction / Protein-Protein Interaction (HPI/PPI) Data
and Visualization**

PATRIC now includes the latest experimental and computational HPI/PPI
data from greater than 15 public repositories, including STRINGDB with a
total of 55 million protein-protein interactions. There is a new
Interactions tab at the Interactions genome, and gene levels, showing
interactions as table and graph. Examples are accessible at 
https://www.patricbrc.org/view/Genome/83332.12#view_tab=interactions and
https://www.patricbrc.org/view/Feature/PATRIC.83332.12.NC_000962.CDS.2507203.2507637.fwd#view_tab=interactions&filter=false

**Compare Region Viewer**

PATRIC has a new Compare Region Viewer that displays flanking regions of
user selected genomes for a particular gene.  This is a
re-implementation of the original SEED Compare Region Viewer using
JavaScript and PattyFams. An example is accessible
at \ https://www.patricbrc.org/view/Feature/RefSeq.83332.12.NC_000962.CDS.2726806.2727339.fwd#view_tab=compareRegionViewer

**Advanced Search Enhancements**

PATRIC has enhanced the Global Search to allow users to search for “all”
or “any” of the search terms and searching for exact terms. The option
of “Any exact terms” is particularly useful for searching using a list
of gene or genome IDs. The Global Search is available at the top right
of any page in PATRIC.

**ID Mapper Tool**

The new PATRIC ID Mapper Tool uses UniProt ID Mapping data to allows
users to enter a list of PATRIC IDs and map them to corresponding
external database identifiers, or vice versa.  The tool is accessible at
https://www.patricbrc.org/app/IDMapper.
