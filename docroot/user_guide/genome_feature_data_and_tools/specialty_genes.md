# Specialty Genes

## Specialty Genes Overview

Specialty Genes refers to the special classes of genes that are of
particular interest to infectious disease researchers, such as
antibiotic resistance genes, virulence factors, drug targets, and human
homologs.

For each specialty genes class, PATRIC:

-   Collects reference gene sets from popular and community recognized
    external databases, many of which are manually curated based on
    literature.

-   Creates our own database of manually curated reference gene sets
    based on literature, as needed, to provide more accurate and
    comprehensive information for NIAID select pathogens.

-   As part of genome annotation, maps reference genes to their homologs
    based on high sequence similarity using BLASTP, and thus, providing
    consistent annotation of specialty genes across all bacterial
    genomes.

-   Makes specialty genes accessible and usable by providing specialized
    analysis and search tools to allow researchers to quickly select
    potential targets for the development of drugs, vaccines, and
    therapeutics.

### Classes and Data Sources of Specialty Genes in PATRIC

-   Antibiotic Resistance Genes: Antibiotic Resistance refers to the
    ability of bacteria to develop resistance to antibiotics through
    gene mutation or acquisition of antibiotic resistance genes. We have
    integrated and mapped known antibiotic resistance genes from the
    following sources:
    -   [ARDB - Antibiotic Resistance Genes Database](http://ardb.cbcb.umd.edu/)
    -   [CARD - The Comprehensive Antibiotic Resistance Database](http://arpcard.mcmaster.ca/)

-   Drug Targets: Drug Targets are proteins being targeted by known,
    approved, or experimental small molecule drugs. We have integrated
    and mapped such drug targets from the following sources:
    -   [DrugBank](http://www.drugbank.ca/)
    -   [TTD – Therapeutic Targets Database](http://bidd.nus.edu.sg/group/TTD/ttd.asp)

-   Human Homologs: Human Homologs are the bacterial proteins that share
    high sequence similarity with human proteins. We have integrated and
    mapped proteins from the Reference Human Genome available at NCBI
    RefSeq .
    -   [Proteins from the Reference Human Genome at NCBI RefSeq](http://www.ncbi.nlm.nih.gov/assembly/GCF_000001405.26)

-   Virulence Factors: Virulence Factors are the gene products that
    enable bacteria to establish itself on or within a host organism and
    enhance its potential to cause disease. We have integrated and
    mapped virulence factor genes from the following sources:
    -   [VFDB](http://www.mgc.ac.cn/VFs/main.htm)
    -   [Victors](http://www.phidias.us/victors/)
    -   [PATRIC\_VF](http://patricbrc.org/portal/portal/patric/SpecialtyGeneSource?source=PATRIC_VF)

*\*Note:* PATRIC\_VF is a manually curated virulence factor database,
which contains the genes identified as playing a role in virulence in
certain organisms. Each PATRIC\_VF gene is linked to one or more journal
articles that establish its virulence based on experimental evidence.
For more details, see [PATRIC\_VF FAQs.](http://enews.patricbrc.org/faqs/patric-curated-virulence-factors-faqs/)

------------------------------------------------------------------------

#### ***Mapping Specialty Genes to PATRIC Proteins***

For each class of specialty genes, we gather reference gene sets from
the data sources described above. We create specialized BLAST databases
using protein sequences for each reference gene set, which are then used
as part of the genome annotation pipeline. For each genome in PATRIC, we
take all predicted protein sequences and search them against each of the
specialized BLAST databases using BLASTP.

The top BLAST hits are parsed and filtered based on sequence identity
and sequence coverage using the following criteria:

*(%Query coverage &gt;=80 OR %Subject coverage &gt;=80) AND %Identity
&gt;=80*

For identifying Human Homologs, we use:

*(%Query coverage &gt;=50 OR %Subject Coverage &gt;=50) AND %Identity
&gt;=50*

### Evidence Field

All the BLAST hits that pass the above-mentioned similarity criteria are
further classified as follows using field “Evidence”.

-   *Literature:* For any BLAST hit, if the query and the subject genes
    are the same, i.e. the same genes in the same genome based on locus
    tag or some other identifier match, we designate the Evidence as
    “Literature”. This means that there is direct literature evidence
    describing the gene in question, which probably characterizes the
    gene based on experimental evidence.
    -   *\*Note:* even when a hit is classified as “Literature”,
        sequence coverage and/or percent identity for the sequence
        similarity could still be below 100%, because of the differences
        in the start site of the same gene as predicted by different
        annotation systems.

-   *BLASTP:* For all BLAST hits that are not classified as
    “Literature”, we designate the Evidence as “BLASTP”. This means that
    the gene in question is highly similar to a specialty gene described
    in one of the source databases. However, the reference gene may or
    may not be exactly the same gene and/or in the same genome.

### Accessing Specialty Genes on the PATRIC Website

At PATRIC, you can access specialty genes and related information in the
following ways:

-   Using the [Specialty Genes Data Summary](https://www.patricbrc.org/view/DataType/SpecialtyGenes)
    available under the “Data” Tab in the main navigation along the top
    of the PATRIC site. Here you can view summaries of selected genomes,
    related tools and tutorials, and diagrams of how we curate, map, and
    integrate Specialty Genes.
-   Via the “Specialty Genes” Tab on any taxon or genome page. Here
    you’ll find a pre-scoped Specialty Genes List.
-   As a tabular summary at the bottom of any genome page.
-   As a tabular summary entitled Special Properties at the bottom of a
    gene page.
-   Using the "Specialty Genes" option in the Global Search.

### Specialty Gene List and Related Filters

The Specialty Gene List provides the following information:

-   Information about PATRIC genes, such as Genome Name, PATRIC and
    RefSeq Locus Tags, Gene Names, and Products.
-   Information about the matching specialty gene in the reference
    database, such as Property, Source Database Name, Source ID,
    Classification, and PubMed references. Source IDs are linked to the
    corresponding pages on the Source Database websites where you can
    access more information. PubMed links take you to the corresponding
    references lists at PubMed.
-   Summaries of sequence similarity from BLASTP hit, such as Percent
    Query Coverage, Percent Subject Coverage, and Percent Identity.

The Specialty Gene List can be filtered using the options from the
filter panel which can be opened from the icon at the top right of the
table:

-   *Filter by Keyword*: Search using any keywords related to the
    Organism Name, Gene Name, Locus Tag, or Gene Product and find
    matching specialty genes.
-   *Filter by Property:* Select one or more classes of specialty genes,
    such as Antibiotic Resistance Genes, or Virulence Factors.
-   *Filter by Source:* Select one or more source databases to see genes
    similar to the reference genes from those databases.
-   *Filter by Evidence:* Hits designated as “Literature” imply that the
    query and the subject genes are the same, i.e. the same genes in the
    same genome based on locus tag or some other identifier match,
    however, there may be some differences in the start site. It means
    that there is direct literature evidence describing the gene in
    question, which probably characterizes the gene based on
    experimental evidence. All other hits designated as “BLASTP” imply
    that the gene in question is highly similar to a reference gene
    described in one of the source databases. However, the reference
    gene may or may not be exactly the same gene and/or in the same
    genome.
