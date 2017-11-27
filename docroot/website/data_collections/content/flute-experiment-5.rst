===================
Flute Experiment 5
===================

TnSeq datasets for 10 knockouts in Mtb
======================================

In this experiment, knockout strains for 10 genes in *Mycobacterium
tuberculosis* H37Rv and assayed by TnSeq to identify conditional
essentials (compared to WT; using the resampling statistical method in
Transit). The target genes (knockedout) are: Rv3594, Rv3717, Rv3811,
Rv0307c, Rv3916c, Rv0950, Rv1096, Rv3684, Rv0954, and Rv3671c.

The raw sequence data was deposited in SRA under accession number
SRP101586.

For each target, there are 1-4 replicates, as indicated in the
spreadsheet below

`SRA_metadata_U19_TnSeq_Mar2017.xlsx <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/SRA_metadata_U19_TnSeq_Mar2017.xlsx>`_

**TnSeq Datasets:**

The .wig files below for each sample contain the transposon insertion
counts at TA sites. The reference sequence for the coordinates was `NC_000962.3 <https://www.ncbi.nlm.nih.gov/protein/NC_000962.3>`_

+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| **ID**   | **Title**                                           | **Wig file**                                                                                                        |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 1        | TnSeq library of knockout of Rv3594                 | `delta\_Rv3594\_TnSeq.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/delta_Rv3594_TnSeq.wig>`__        |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 2        | TnSeq library of knockout of Rv3717                 | `delta\_Rv3717\_TnSeq\_1.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/delta_Rv3717_TnSeq_1.wig>`__   |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 3        | TnSeq library of knockout of Rv3811                 | `delta\_Rv3811\_TnSeq.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/delta_Rv3811_TnSeq.wig>`__        |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 4        | TnSeq library of knockout of Rv0307c, replicate 1   | `Rv0307c\_day0\_rep1.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/Rv0307c_day0_rep1.wig>`__          |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 5        | TnSeq library of knockout of Rv0307c, replicate 2   | `Rv0307c\_day0\_rep2.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/Rv0307c_day0_rep2.wig>`__          |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 6        | TnSeq library of knockout of Rv3916c, replicate 1   | `Rv3916c\_day0\_rep1.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/Rv3916c_day0_rep1.wig>`__          |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 7        | TnSeq library of knockout of Rv3916c, replicate 2   | `Rv3916c\_day0\_rep1.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/Rv3916c_day0_rep2.wig>`__          |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 8        | TnSeq library of knockout of Rv0950                 | `TnSeq\_Mtb\_Rv0950ko.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/TnSeq_Mtb_Rv0950ko.wig>`__        |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 9        | TnSeq library of knockout of Rv1096                 | `TnSeq\_Mtb\_Rv1096ko.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/TnSeq_Mtb_Rv1096ko.wig>`__        |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 10       | TnSeq library of knockout of Rv3684                 | `TnSeq\_Mtb\_Rv3684ko.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/TnSeq_Mtb_Rv3684ko.wig>`__        |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 11       | TnSeq library of knockout of Rv0954, replicate 1    | `delta\_Rv0954\_1.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/delta_Rv0954_1.wig>`__                |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 12       | TnSeq library of knockout of Rv0954, replicate 2    | `delta\_Rv0954\_2.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/delta_Rv0954_2.wig>`__                |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 13       | TnSeq library of knockout of Rv3671c, replicate 1   | `marP1.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/marP1.wig>`__                                    |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 14       | TnSeq library of knockout of Rv3671c, replicate 2   | `marP2.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/marP2.wig>`__                                    |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 15       | TnSeq library of knockout of Rv3671c, replicate 3   | `marP3.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/marP3.wig>`__                                    |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+
| 16       | TnSeq library of knockout of Rv3671c, replicate 4   | `marP4.wig <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/marP4.wig>`__                                    |
+----------+-----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------+

**Conditional Essentials:**

The target (KO) genes below link to .dat files that provide lists of
associated conditional essentials. The significant hits are those with
Adjusted\_pval<0.05.

+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Target (KO) Gene**   | **Conditional Essentials**                                                                                                                                          |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv3594                 | `resampling\_H37Rv\_vs\_delta\_Rv3594\_TTR.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_H37Rv_vs_delta_Rv3594_TTR.dat>`__                 |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv3717                 | `resampling\_H37Rv\_vs\_delta\_Rv3717\_TTR.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_H37Rv_vs_delta_Rv3717_TTR.dat>`__                 |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv3811                 | `resampling\_H37Rv\_vs\_delta\_Rv3811\_TTR.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_H37Rv_vs_delta_Rv3811_TTR.dat>`__                 |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv0307c                | `resampling\_H37Rv\_Rv0307c\_day0\_s10000\_pc0.00.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_H37Rv_Rv0307c_day0_s10000_pc0.00.dat>`__   |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv3916c                | `resampling\_H37Rv\_Rv3916c\_day0\_s10000\_pc0.00.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_H37Rv_Rv3916c_day0_s10000_pc0.00.dat>`__   |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv0950                 | `resampling\_H37Rv\_Rv0950\_day0\_s10000\_pc0.00.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_H37Rv_Rv0950_day0_s10000_pc0.00.dat>`__     |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv1096                 | `resampling\_H37Rv\_Rv1096\_day0\_s10000\_pc0.00.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_H37Rv_Rv1096_day0_s10000_pc0.00.dat>`__     |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv3684                 | `resampling\_H37Rv\_Rv3684\_day0\_s10000\_pc0.00.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_H37Rv_Rv3684_day0_s10000_pc0.00.dat>`__     |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv0954                 | `resampling\_WT\_Rv0954\_s10000\_pc0.00.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_WT_Rv0954_s10000_pc0.00.dat>`__                      |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Rv3671c                | `resampling\_WT\_marP\_s10000\_pc0.00\_1.dat <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/resampling_WT_marP_s10000_pc0.00_1.dat>`__                     |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+

**Methods references:**

#. Long, J.E., DeJesus, M., Ward, D., Baker, R.E., Ioerger, T.R. and
   Sassetti, C.M. (2015). Identifying essential genes in *Mycobacterium
   tuberculosis* by global phenotypic profiling. in: Methods in
   `*Molecular Biology: Gene
   Essentiality* <http://www.springer.com/biomed/human+genetics/book/978-1-4939-2397-7>`__,
   (Long Jason Lu, ed.), vol. 1279.
#. DeJesus, M.A., Ambadipudi, C., Baker, R., Sassetti, C., and Ioerger,
   T.R. (2015). TRANSIT a Software Tool for Himar1 TnSeq Analysis. *PLOS
   Computational Biology*, 11(10):e1004401. `PMID
   26447887 <https://www.ncbi.nlm.nih.gov/pubmed/26447887>`__.

**Downloads:**

All files are available from
FTP:\ ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_5/.

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </div>
