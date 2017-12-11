==============================================
PATRIC September 2015 Data and Website Release
==============================================


:date:   2015-10-01T09:33:17+00:00

**AMR Metadata**

In this release, we have added additional antimicrobial resistance
phenotype related metadata for 949 genomes. The AMR panel data was
primarily provided by the NIAID Genomic Centers for Infectious Diseases,
which was incorporated into PATRIC after a comprehensive manual curation
process.

Below is the summary of the top bacterial genera with AMR metadata.

.. raw:: html

   <center>

.. raw:: html

   </center>

.. raw:: html

   <table>

.. raw:: html

   <tr>

.. raw:: html

   <td style="text-align: center;" width="250">

Genus

.. raw:: html

   </td>

.. raw:: html

   <td style="text-align: center;" width="250">

Number of genomes with AMR metadata

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td style="text-align: center;" width="250">

Streptococcus

.. raw:: html

   </td>

.. raw:: html

   <td style="text-align: center;" width="250">

3210

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td style="text-align: center;" width="250">

Mycobacterium

.. raw:: html

   </td>

.. raw:: html

   <td style="text-align: center;" width="250">

1338

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td style="text-align: center;" width="250">

Staphylococcus

.. raw:: html

   </td>

.. raw:: html

   <td style="text-align: center;" width="250">

620

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td style="text-align: center;" width="250">

Klebsiella

.. raw:: html

   </td>

.. raw:: html

   <td style="text-align: center;" width="250">

259

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td style="text-align: center;" width="250">

Acinetobacter

.. raw:: html

   </td>

.. raw:: html

   <td style="text-align: center;" width="250">

236

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td style="text-align: center;" width="250">

Pseudomonas

.. raw:: html

   </td>

.. raw:: html

   <td style="text-align: center;" width="250">

125

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td style="text-align: center;" width="250">

Enterobacter

.. raw:: html

   </td>

.. raw:: html

   <td style="text-align: center;" width="250">

65

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td style="text-align: center;" width="250">

Escherichia

.. raw:: html

   </td>

.. raw:: html

   <td style="text-align: center;" width="250">

50

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </table>

** **\ All AMR metadata incorporated thus far is available on the FTP
site for
`download <ftp://ftp.patricbrc.org/BRC_Mirrors/AMR/PATRIC_genomes_AMR.xlsx>`__.
In addition, we have also created a `special FTP
directory <ftp://ftp.patricbrc.org/patric2/current_release/AMR_genome_sets>`__
where we have published 11 genus-specific AMR genome sets that contain
more than 100 antimicrobial resistant and susceptible genomes for a
given antibiotic. The goal of this directory is to provide easy access
to the balanced AMR genome sets to users interested in building AMR
Classifiers.

**Other Metadata Updates**

** **\ Additional metadata updates include incorporation of additional
clinical metadata from the NIAID Genomic Centers for Infectious
Diseases; addition of accession numbers for Assembly (6560), BioProject
(2440), BioSample (6619), and GenBank (3133); genome name changes (698)
to include strain names; and consolidation of some potentially redundant
metadata fields.

**New PATRIC Genus-specific and Cross-genera Protein Families**

We have computed new genus-specific protein families (PLfams) and
cross-genera protein families (PGfams) for all the public genomes in
PATRIC. These protein families cover almost all of the proteins in the
current public genomes (~100% protein coverage) to support more
comprehensive comparative analysis.

The protein families are computed using the procedure described below:

-  All the proteins from public genomes currently available in PATRIC
   are assigned function based on the most recent signature k-mers. For
   all the proteins with identical functions, a similarity matrix is
   computed based on the number of signature k-mers they have in common,
   divided by average protein length for every pair of proteins. This
   k-mer similarity matrix is then processed using MCL algorithm, which
   forms one or more protein clusters based on similarity among the
   members.

   -  The genus-specific protein families are computed using only
      proteins within a genus and more stringent criteria (MCL inflation
      = 3.0). This provides higher sequence similarity and better
      specificity while performing within-genus/species or close strain
      comparisons.
   -  The cross-genera protein families are computed by clustering
      representative proteins from the genus-specific families with
      slightly relaxed criteria (MCL inflation = 1.1). This allows
      cross-genera or distant homologs to cluster together, which is
      necessary to support cross-genera comparative analysis across all
      microbial genomes.

The new protein families are accessible through the Genome and Gene
Overview webpages and through the Protein Family Sorter tool. The
Protein Family Sorter now allows users to perform comparative analysis
using PLfams, PGfams, or FIGfams.

**Annotation Updates**

This release features complete functional annotation update of all the
public genomes in PATRIC. All the proteins from the public genomes were
rerun through the latest version of functional annotation pipeline to
assign functions based on the most up-to-date manually curated
annotations of the subsystems.

Please note that private genomes annotated by PATRIC users have not
received any protein family or function updates. We are currently
working on updating the PATRIC annotation service to support the
annotation of new protein families and functions. We expect this update
to be available in our next release.

All of the data download files on the FTP site that contain PATRIC
annotations have been updated to provide the latest annotations.

**Website Minor Bug Fixes**

This release also features website bug fixes, minor enhancements, and
performance improvements. The most notable change in the website
functionality is the incorporation of the new protein families (PLfams
and PGfams) on the Genomes overview, Gene overview, and Protein Family
Sorter webpages.
