:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/20161202-patric-november-release-features-over-9000-new-genomes-host-genomes-and-annotations-essential-gene-predictions-command-line-interface-rna-seq-service-enhancements-and-other-updates.rst

=========================================================================================================================================================================================
PATRIC November Release features over 9000 New Genomes, Host Genomes and Annotations, Essential Gene Predictions, Command Line Interface, RNA-Seq Service Enhancements and Other Updates.
=========================================================================================================================================================================================

.. feed-entry::
   :date: 2016-12-02

**New Genomes**

In this release, PATRIC has added 9,136 new genomes, bringing the total
number of genomes in PATRIC to over 89,000. Total 174 genomes, which
were of low quality or obsolete, were deleted from PATRIC. In addition,
names of 1,633 genomes were revised to include strain names to make them
more informative. The full list of available bacterial genomes can be
accessed from the `Genomes Tab for all
bacteria <https://www.patricbrc.org/portal/portal/patric/GenomeList?cType=taxon&cId=2&dataSource=&displayMode=&pk=&kw=>`__.
on the old Production site and  `Genomes tab for all
bacteria <https://www.patricbrc.org/view/Taxonomy/2#view_tab=genomes>`__ 
on the Beta website.

**Protein Family and Annotation Updates**

This release features complete functional re-annotation of all public
genomes in PATRIC.  The functional re-annotation of the genomes is
carried out to propagate recent annotation changes made by PATRIC
curators and to incorporate latest knowledge from the literature. During
re-annotation process, the structural annotations (i.e. genomic
features, gene locations, and their sequences) remain unchanged.
However, all protein-coding genes (CDS) are run again through the latest
annotation pipeline to reassign their functions. Changes in function may
also lead to corresponding changes in the pathway assignments. The
PATRIC genus-specific (PLFams) and cross-genera (PGFams) families have
also been updated to reflect recent changes in the protein annotations.
The protein family identifiers were preserved when the composition of
the new families were mostly the same as that of old families.

**Host Genomes and Annotations**

PATRIC now has a set of representative host genomes in PATRIC, with
annotations.  These include *Homo sapiens* (human), *Mus musculus*
(mouse), *Macaca mulatta* (Rhesus macaque monkey), Rattus norvegicus
(rat), *Sus scrofa* (pig), *Mustela putorius furo* (ferret), *Danio
rerio* (zebrafish), *Gallus gallus* (chicken), *Drosophila melanogaster*
(fruit fly), and *Caenorhabditis elegans* (roundworm). These genomes are
available in PATRIC as `an option in the Organisms
menu <https://www.patricbrc.org/view/Taxonomy/2759#view_tab=genomes>`__ on
the Beta website.

**AMR Gene Annotations**

With this release, PATRIC provides additional AMR gene annotations,
which are propagated from set of high quality AMR genes manually curated
by the PATRIC Team. These curated AMR genes correspond to 25 AMR
subsystems, covering 227 unique AMR functional roles. Additional
information is available
`here <http://enews.patricbrc.org/4974/patric-antimicrobial-resistance-amr-gene-curation/>`__.
The curated AMR gene functions have been consistently projected to more
than 1.6M genes from >71,000 public bacterial genomes currently
available in PATRIC. Projected AMR gene annotations are available under
the `Specialty Genes Tab on the website, with filters
Property=Antibiotic Resistance and
Source=PATRIC <https://www.patricbrc.org/view/SpecialtyGeneList/?keyword(*)#view_tab=specialtyGenes&filter=and(or(eq(property,%22Antibiotic%20Resistance%22)),eq(source,%22PATRIC%22))>`__ on
the Beta website.

**AMR Classifier Enhancements:**

PATRIC has increased the set of AdaBoost-based machine learning AMR
classifiers that are currently available in the PATRIC Genome Annotation
Service by using new genomes and associated AMR resistance data. The
preexisting set of classifiers have also been updated. This is an
ongoing enhancement process as we bring in additional genomes into
PATRIC that have AMR resistance data.  The PATRIC Genome Annotation
Service is available as `an option in the Services
menu <https://www.patricbrc.org/app/Annotation>`__.

**Essential Gene Predictions**

PATRIC now provides predicted of essential genes for 7923 Reference and
Representative genomes. These essential genes were predicted using
flux-balance analysis (FBA) wherein a genome-scale metabolic model is
used to predict the growth conditions for an organism by simulating the
simultaneous production of all the small molecule building blocks of
biomass (e.g. amino acids, cofactors, nucleotides) from compounds
available in the growth media (e.g. sugar, vitamins, amino acids).
Additional information about this process is available from
http://www.nature.com/nbt/journal/v28/n3/abs/nbt.1614.html. The
essential gene predictions are available at PATRIC under `the Specialty
Genes Tab on the website, with filters Property=Essential Gene and
Source=PATRIC <https://www.patricbrc.org/view/SpecialtyGeneList/?keyword(*)#view_tab=specialtyGenes&filter=and(eq(property,%22Essential%20Gene%22),or(eq(source,%22PATRIC%22)))>`__ on
the Beta website.

**Command Line and Application Programming Interfaces (CLI and API)**

The initial version of the PATRIC CLI/API is now available.  It allows
users to programmatically batch upload data to their PATRIC workspace,
invoke services (e.g., Assembly, Annotation), and download the results. 
The CLI/API can be downloaded as a dmg from
https://github.com/PATRIC3/PATRIC-distribution/releases.

**RNA-Seq Analysis Service Enhancements:**

The PATRIC RNA-Seq Service is now enhanced to support RNA-Seq data using
the host genomes that we currently have in PATRIC (human, mouse, monkey,
rat, pig, ferret, zebrafish, chicken, fruit fly, and roundworm). The
PATRIC RNA-Seq Analysis Service is available as `an option in the
Services menu <https://www.patricbrc.org/app/Rnaseq>`__.
