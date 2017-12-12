:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/20160331-patric-antimicrobial-resistance-amr-gene-curation.rst

===================================================
PATRIC Antimicrobial Resistance (AMR) Gene Curation
===================================================

.. feed-entry::
   :date: 2016-03-31

PATRIC has undertaken an antimicrobial resistance (AMR) curation effort
with the goal of providing PATRIC users with the ability to rapidly
recognize and project known AMR related genome features to new genomes
in an automated fashion and to use comparative genomics approaches for
the discovery of new resistance mechanisms.

**Specific Aims:**

-  Catalog published AMR related genes in the 22 genera of infectious
   disease organisms, providing high quality detailed annotations of all
   AMR determinants
-  Enable rapid recognition and automated projection of known AMR
   related genome features to new genomes
-  Support classification of genomes as resistant or susceptible
-  Enable prediction and discovery of novel resistance mechanisms

The ongoing **AMR curation** enables this through the development and of
a comprehensive up-to-date collection of AMR determinants and genomic
variations.  These structured collections will be used in several ways
including automated **propagation of AMR-related annotations** that will
significantly enhance AMR analysis for PATRIC users.

Two approaches are currently under construction to project AMR gene
annotations to a new genome. First, once a new AMR-related function has
been entered into the database, it will be recognized by our k-mer-based
projection software, and new genomes with the gene will be annotated
with that function (1-3). Secondly, when a genome that is being
annotated is very similar to one of the reference genomes in PATRIC, the
AMR annotations from the reference genome will be directly applied to
the new genome, when appropriate to do so.

The database that will drive this annotation module is currently under
construction.  It is structured as a collection of dedicated
**AMR-related Subsystems** that are being added to the genome annotation
engine underlying the PATRIC database. Subsystems connect encoded AMR
determinants to relevant literature, describe mechanisms of action (if
available), and lay the basis for variation analysis.  Approximately
half of new Subsystems required to encode known AMR-related genes and
gene products are in place. An Excel spreadsheet with these data is
available
:download:`here <../files/201603/PATRIC-AMR-Gene-Curation-2016-03-31.xlsx>`.
 Together they cover 265 unique Functional roles (isofunctional protein
families), each corresponding to a specific AMR determinant encoded
across a representative set of ~1000 diverse prokaryotic genomes.

Curation thus far has focused on encoding the following mechanisms of
drug resistance (shown below): outer membrane porins, multidrug efflux
mechanisms, and capsular and extracellular polysacchrides (as the
balance of drug influx and efflux is the first line of microbial defense
against antibiotics).  In addition, all types of tetracycline resistance
have been captured and work on beta-lactamases has started.  The
remaining AMR determinants will be encoded during the remainder the
project.

**Common mechanisms of drug resistance**

-  **Efflux pumps**

   -  Up-regulation, often via mutations in promotors, operators

-  ** Outer membrane proteins/porins (influx)**

   -  Inactivation via loss of function mutations, deletions,
      truncations

-  ** Drug modifying enzymes**

   -  Ribosome protection (TetR) proteins
   -  β-lactamases
   -  Aminoglycoside-modifying enzymes
   -  RNA methyltransferases

-  ** Target modifications**

   -  Gyrase modifications (gyrA/B, parC/E mutations)
   -  Ribosomal subunit, rRNA mutations
   -  mecA – PBP2a (MRSA)

**References**

1. Brettin T, Davis JJ, Disz T, Edwards RA, Gerdes S, Olsen GJ, Olson R,
   Overbeek R, Parrello B, Pusch GD, Shukla M, Thomason JA 3rd, Stevens
   R, Vonstein V, Wattam AR, Xia F. RASTtk: a modular and extensible
   implementation of the RAST algorithm for building custom annotation
   pipelines and annotating batches of genomes. Sci Rep. 2015 Feb
   10;5:8365. doi: 10.1038/srep08365. PMID:
   `25666585 <http://www.ncbi.nlm.nih.gov/pubmed/?term=25666585>`__.
   PMCID: \ `PMC4322359 <http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4322359/>`__.
2. Overbeek R, Olson R, Pusch GD, Olsen GJ, Davis JJ, Disz T, Edwards
   RA, Gerdes S, Parrello B, Shukla M, Vonstein V, Wattam AR, Xia F,
   Stevens R. The SEED and the Rapid Annotation of microbial genomes
   using Subsystems Technology (RAST). Nucleic Acids Res. 2014
   Jan;42(Database issue):D206-14. doi: 10.1093/nar/gkt1226. PMID:
   `24293654 <http://www.ncbi.nlm.nih.gov/pubmed/?term=24293654>`__.
   PMCID: \ `PMC3965101 <http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3965101/>`__.
3. Davis JJ, Gerdes S, Olsen GJ, Olson R, Pusch GD, Shukla M, Vonstein
   V, Wattam AR, Yoo H. PATtyFams: Protein Families for the Microbial
   Genomes in the PATRIC Database. Front Microbiol. 2016 Feb 8;7:118.
   doi: 10.3389/fmicb.2016.00118. eCollection 2016. PMID:
   `26903996 <http://www.ncbi.nlm.nih.gov/pubmed/?term=26903996>`__.
   PMCID:
   `PMC4744870 <http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4744870/>`__.
