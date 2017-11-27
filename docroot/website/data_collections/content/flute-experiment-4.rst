
===================
Flute Experiment 4
===================

Statistical analysis of genetic interactions in Tn-Seq data
===========================================================

**Publication:** `PMID
28334803 <https://www.ncbi.nlm.nih.gov/pubmed/28334803>`_

Tn-Seq is an experimental method for probing the functions of genes
through construction of complex random transposon insertion libraries
and quantification of each mutant's abundance using next-generation
sequencing. An important emerging application of Tn-Seq is for
identifying genetic interactions, which involves comparing Tn mutant
libraries generated in different genetic backgrounds (e.g. wild-type
strain versus knockout strain). Several analytical methods have been
proposed for analyzing Tn-Seq data to identify genetic interactions,
including estimating relative fitness ratios and fitting a generalized
linear model. However, these have limitations which necessitate an
improved approach. We present a hierarchical Bayesian method for
identifying genetic interactions through quantifying the statistical
significance of changes in enrichment. The analysis involves a four-way
comparison of insertion counts across datasets to identify transposon
mutants that differentially affect bacterial fitness depending on
genetic background. Our approach was applied to Tn-Seq libraries made in
isogenic strains of *Mycobacterium tuberculosis* lacking three different
genes of unknown function previously shown to be necessary for optimal
fitness during infection. By analyzing the libraries subjected to
selection in mice, we were able to distinguish several distinct classes
of genetic interactions for each target gene that shed light on their
functions and roles during infection.

The raw sequence data was deposited in SRA under accession number
SRP081827.

For each KO strain, there were 2 replicates in-vitro ("day 0 in mice")
and 3 replicates in-vivo (day 32 in mice). The Excel file below provides
definitions of each sample number, e.g., U19_73 in column M is "TnSeq
library of wildtype infected in mice, day 0, replicate 1" in column D.

`SRA_metadata-TnSeq-GI-paper.xlsx <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_4/SRA_metadata-TnSeq-GI-paper.xlsx>`_

**TnSeq Datasets:**

+-----------------------+-----------------------+-----------------------+
| **ID**                | **Title**             | **Wig file**          |
+-----------------------+-----------------------+-----------------------+
| 1                     | TnSeq library of      | `U19_73.wig <ftp://ft |
|                       | wildtype infected in  | p.patricbrc.org/BRC_M |
|                       | mice, day 0,          | irrors/FLUTE/Experime |
|                       | replicate 1           | nt_4/U19_73.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 2                     | TnSeq library of      | `U19_74.wig <ftp://ft |
|                       | wildtype infected in  | p.patricbrc.org/BRC_M |
|                       | mice, day 0,          | irrors/FLUTE/Experime |
|                       | replicate 2           | nt_4/U19_74.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 3                     | TnSeq library of      | `U19_75.wig <ftp://ft |
|                       | wildtype infected in  | p.patricbrc.org/BRC_M |
|                       | mice, day 32,         | irrors/FLUTE/Experime |
|                       | replicate 1           | nt_4/U19_75.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 4                     | TnSeq library of      | `U19_76.wig <ftp://ft |
|                       | wildtype infected in  | p.patricbrc.org/BRC_M |
|                       | mice, day 32,         | irrors/FLUTE/Experime |
|                       | replicate 2           | nt_4/U19_76.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 5                     | TnSeq library of      | `U19_77.wig <ftp://ft |
|                       | wildtype infected in  | p.patricbrc.org/BRC_M |
|                       | mice, day 32,         | irrors/FLUTE/Experime |
|                       | replicate 3           | nt_4/U19_77.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 6                     | TnSeq library of      | `U19_81.wig <ftp://ft |
|                       | knockout of Rv2680    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 0, replicate 1        | nt_4/U19_81.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 7                     | TnSeq library of      | `U19_82.wig <ftp://ft |
|                       | knockout of Rv2680    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 0, replicate 2        | nt_4/U19_82.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 8                     | TnSeq library of      | `U19_83.wig <ftp://ft |
|                       | knockout of Rv2680    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 32, replicate 1       | nt_4/U19_83.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 9                     | TnSeq library of      | `U19_84.wig <ftp://ft |
|                       | knockout of Rv2680    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 32, replicate 2       | nt_4/U19_84.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 10                    | TnSeq library of      | `U19_85.wig <ftp://ft |
|                       | knockout of Rv2680    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 32, replicate 3       | nt_4/U19_85.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 11                    | TnSeq library of      | `U19_86.wig <ftp://ft |
|                       | knockout of Rv1565c   | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 0, replicate 1        | nt_4/U19_86.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 12                    | TnSeq library of      | `U19_87.wig <ftp://ft |
|                       | knockout of Rv1565c   | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 0, replicate 2        | nt_4/U19_87.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 13                    | TnSeq library of      | `U19_88.wig <ftp://ft |
|                       | knockout of Rv1565c   | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 32, replicate 1       | nt_4/U19_88.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 14                    | TnSeq library of      | `U19_89.wig <ftp://ft |
|                       | knockout of Rv1565c   | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 32, replicate 2       | nt_4/U19_89.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 15                    | TnSeq library of      | `U19_90.wig <ftp://ft |
|                       | knockout of Rv1565c   | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 32, replicate 3       | nt_4/U19_90.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 16                    | TnSeq library of      | `U19_91.wig <ftp://ft |
|                       | knockout of Rv1432    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 0, replicate 1        | nt_4/U19_91.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 17                    | TnSeq library of      | `U19_92.wig <ftp://ft |
|                       | knockout of Rv1432    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 0, replicate 2        | nt_4/U19_92.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 18                    | TnSeq library of      | `U19_93.wig <ftp://ft |
|                       | knockout of Rv1432    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 32, replicate 1       | nt_4/U19_93.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 19                    | TnSeq library of      | `U19_94.wig <ftp://ft |
|                       | knockout of Rv1432    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 32, replicate 2       | nt_4/U19_94.wig>`__   |
+-----------------------+-----------------------+-----------------------+
| 20                    | TnSeq library of      | `U19_95.wig <ftp://ft |
|                       | knockout of Rv1432    | p.patricbrc.org/BRC_M |
|                       | infected in mice, day | irrors/FLUTE/Experime |
|                       | 32, replicate 3       | nt_4/U19_95.wig>`__   |
+-----------------------+-----------------------+-----------------------+

**Downloads:**

All files are available from
FTP:\ ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_4/.

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </div>
