===================
Flute Experiment 1
===================

High-Resolution Phenotypic Profiling Defines Genes Essential for Mycobacterial Growth and Cholesterol Catabolism
=================================================================================================================

**Publication:** `PMC3182942 <http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3182942/>`_

The pathways that comprise cellular metabolism are highly
interconnected, and alterations in individual enzymes can have
far-reaching effects. As a result, global profiling methods that measure
gene expression are of limited value in predicting how the loss of an
individual function will affect the cell. In this work, we employed a
new method of global phenotypic profiling to directly define the genes
required for the growth of *Mycobacterium tuberculosis*. A combination
of high-density mutagenesis and deep-sequencing was used to characterize
the composition of complex mutant libraries exposed to different
conditions. This allowed the unambiguous identification of the genes
that are essential for Mtb to grow *in vitro*, and proved to be a
significant improvement over previous approaches. To further explore
functions that are required for persistence in the host, we defined the
pathways necessary for the utilization of cholesterol, a critical carbon
source during infection. Few of the genes we identified had previously
been implicated in this adaptation by transcriptional profiling, and
only a fraction were encoded in the chromosomal region known to encode
sterol catabolic functions. These genes comprise an unexpectedly large
percentage of those previously shown to be required for bacterial growth
in mouse tissue. Thus, this single nutritional change accounts for a
significant fraction of the adaption to the host. This work provides the
most comprehensive genetic characterization of a sterol catabolic
pathway to date, suggests putative roles for uncharacterized virulence
genes, and precisely maps genes encoding potential drug targets.

In order to precisely define the genes that are important for the growth
of Mtb, we used highly parallel Illumina sequencing to characterize
transposon libraries. This approach achieves single base pair resolution
of insertion sites in very complex libraries, resulting in the precise
identification of essential open reading frames. Furthermore, the depth
of sequencing that is possible allowed the relative abundance of
individual mutants to be accurately assessed in libraries grown under
different conditions. Using the latter approach, we comprehensively
defined the pathways required for the bacterium to grow on cholesterol,
a critical nutrient during infection. These previously ill-defined
pathways account for an unexpectedly large fraction of the genes
required for survival in animal models of TB, providing new functional
insight into the adaptation to the host environment.

| Conditions: grown *in vitro* (minimal media, liquid culture (as
  opposed to plates), as described in the paper, supplemented with
  either 0.1% glycerol or 0.01% cholesterol as a carbon source)
| Library: This TnSeq library was prepared in the Sassetti lab by Jen
  Griffin in 20xx using Himar1 transposon and *M. tuberculosis* H37Rv as
  a parental strain.
| Transposon used: Himar1
| Protocol for library preparation: Himar1 transfection as described in
  paper
| Protocol for TnSeq sample preparation: nested PCR, as described in
  paper
| Protocol for sequencing: XX bp paired-end reads on Illumina GAII
| Protocol for data processing: mapped reads to reference genome using
  SOAP; reported as raw read counts at TA dinucleotides
| Reference Genome: *M. tuberculosis* H37Rv (GenBank refseq accession
  number: NC_000962.2)
| Experimenter/Researcher/Owner of Data: Jen Griffin
| PI/Lab: Chris Sassetti, UMass Med School
| Uploaded/Deposited by: Thomas Ioerger, Texas A&M University

**TnSeq Datasets:**

+-----------------------------------+-----------------------------------+
| **Name**                          | **Wig file**                      |
+-----------------------------------+-----------------------------------+
| Dataset 1                         | `glycerol_H37Rv_rep1.wig <ftp://f |
|                                   | tp.patricbrc.org/BRC_Mirrors/FLUT |
|                                   | E/Experiment_1/glycerol_H37Rv_rep |
|                                   | 1.wig>`__                         |
+-----------------------------------+-----------------------------------+
| Dataset 2                         | `glycerol_H37Rv_rep2.wig <ftp://f |
|                                   | tp.patricbrc.org/BRC_Mirrors/FLUT |
|                                   | E/Experiment_1/glycerol_H37Rv_rep |
|                                   | 2.wig>`__                         |
+-----------------------------------+-----------------------------------+
| Dataset 3                         | `cholesterol_H37Rv_rep1.wig <ftp: |
|                                   | //ftp.patricbrc.org/BRC_Mirrors/F |
|                                   | LUTE/Experiment_1/cholesterol_H37 |
|                                   | Rv_rep1.wig>`__                   |
+-----------------------------------+-----------------------------------+
| Dataset 4                         | `cholesterol_H37Rv_rep2.wig <ftp: |
|                                   | //ftp.patricbrc.org/BRC_Mirrors/F |
|                                   | LUTE/Experiment_1/cholesterol_H37 |
|                                   | Rv_rep2.wig>`__                   |
+-----------------------------------+-----------------------------------+
| Dataset 5                         | `cholesterol_H37Rv_rep3.wig <ftp: |
|                                   | //ftp.patricbrc.org/BRC_Mirrors/F |
|                                   | LUTE/Experiment_1/cholesterol_H37 |
|                                   | Rv_rep3.wig>`__                   |
+-----------------------------------+-----------------------------------+

**Annotations in PATRIC:**

+-----------------------------------+-----------------------------------+
| **LOCUS_TAG**                     | **Annotation in PATRIC**          |
+-----------------------------------+-----------------------------------+
| Rv3193c                           | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=RefSeq.83332.12.NC_0 |
|                                   | 00962.CDS.3560194.3563172.rev>`__ |
+-----------------------------------+-----------------------------------+
| Rv0955                            | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=PATRIC.83332.12.NC_0 |
|                                   | 00962.CDS.1066087.1067445.fwd>`__ |
+-----------------------------------+-----------------------------------+
| Rv2202c                           | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=RefSeq.83332.12.NC_0 |
|                                   | 00962.CDS.2467053.2468027.rev>`__ |
+-----------------------------------+-----------------------------------+
| Rv1130                            | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=PATRIC.83332.12.NC_0 |
|                                   | 00962.CDS.1254609.1256135.fwd>`__ |
+-----------------------------------+-----------------------------------+
| Rv2038c                           | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=PATRIC.83332.12.NC_0 |
|                                   | 00962.CDS.2283723.2284796.rev>`__ |
+-----------------------------------+-----------------------------------+
| Rv2040c                           | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=PATRIC.83332.12.NC_0 |
|                                   | 00962.CDS.2285628.2286491.rev>`__ |
+-----------------------------------+-----------------------------------+
| Rv3005c                           | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=RefSeq.83332.12.NC_0 |
|                                   | 00962.CDS.3363693.3364532.rev>`__ |
+-----------------------------------+-----------------------------------+
| Rv2387                            | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=PATRIC.83332.12.NC_0 |
|                                   | 00962.CDS.2680765.2682018.fwd>`__ |
+-----------------------------------+-----------------------------------+
| Rv3214                            | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=PATRIC.83332.12.NC_0 |
|                                   | 00962.CDS.3591652.3592257.fwd>`__ |
+-----------------------------------+-----------------------------------+
| Rv3283                            | `Feature                          |
|                                   | page <https://www.patricbrc.org/p |
|                                   | ortal/portal/patric/Feature?cType |
|                                   | =feature&cId=PATRIC.83332.12.NC_0 |
|                                   | 00962.CDS.3664958.3665821.fwd>`__ |
+-----------------------------------+-----------------------------------+

**Results Dataset:** `resampling_results_glyc_chol.xlsx <http://brcdownloads.patricbrc.org/BRC_Mirrors/FLUTE/resampling_results_glyc_chol.xlsx>`_

**Conditional Essentials:**

.. raw:: html

   <div>

.. raw:: html

   <div>

.. raw:: html

   <div>

.. raw:: html

   <div>

.. raw:: html

   <div>

The following genes are indicated as conditional essentials based
on statistical analysis (resampling) output using Transit software
(http://saclab.tamu.edu/essentiality/transit/). In this method, for each
ORF (e.g., Rv0001) Transit calculates to determine whether the
essentiality of the gene significantly increase or decreases. The
adjusted p-value uses the Benjamini-Hochberg correction for multiple
tests, with a threshold of <0.05 for significance.

.. raw:: html

   </div>

.. raw:: html

   <div>

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   <div>

**resampling_results_glyc_chol**

.. raw:: html

   </div>

.. raw:: html

   <div>

+-----------------+-----------------+-----------------+-----------------+
| **ORF**         | **log2 FC**     | **q-value**     | **Feature in    |
|                 |                 |                 | PATRIC**        |
+-----------------+-----------------+-----------------+-----------------+
| Rv0362          | -9.05           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.439871.4412 |
|                 |                 |                 | 53.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0485          | -6.2            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.574185.5753 |
|                 |                 |                 | 00.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0999          | 2.54            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1115767.111 |
|                 |                 |                 | 6525.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1130          | -6.6            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1254609.125 |
|                 |                 |                 | 6135.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1287          | 3.19            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1440835.144 |
|                 |                 |                 | 1290.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1807          | 3.23            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2048386.204 |
|                 |                 |                 | 9597.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2691          | 2.88            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3009344.301 |
|                 |                 |                 | 0027.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2936          | 2.25            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3272214.327 |
|                 |                 |                 | 3209.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2938          | 1.82            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3274165.327 |
|                 |                 |                 | 4902.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2942          | 2.12            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3285115.328 |
|                 |                 |                 | 7832.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2945c         | 3.47            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3290624.329 |
|                 |                 |                 | 1304.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3200c         | 3.73            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3572602.357 |
|                 |                 |                 | 3669.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3484          | 4.46            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3903171.390 |
|                 |                 |                 | 4616.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3494c         | -7.25           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3911675.391 |
|                 |                 |                 | 3369.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3496c         | -4.84           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3914531.391 |
|                 |                 |                 | 5886.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3497c         | -5.2            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3915883.391 |
|                 |                 |                 | 6956.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3526          | -8.69           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3962544.396 |
|                 |                 |                 | 3599.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3540c         | -8.42           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3979499.398 |
|                 |                 |                 | 0659.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3544c         | -8.1            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3983125.398 |
|                 |                 |                 | 4144.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3551          | -9.19           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3989896.399 |
|                 |                 |                 | 0774.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3553          | -7.98           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3991621.399 |
|                 |                 |                 | 2688.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3560c         | -7.29           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.4000432.400 |
|                 |                 |                 | 1589.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3571          | -10.44          | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.4012417.401 |
|                 |                 |                 | 3493.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3696c         | 6.67            | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.4138202.413 |
|                 |                 |                 | 9755.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1129c         | -5.53           | 0.0148          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1253074.125 |
|                 |                 |                 | 4435.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3568c         | -8.06           | 0.0148          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.4009297.401 |
|                 |                 |                 | 0199.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3569c         | -7.87           | 0.0148          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.4010196.401 |
|                 |                 |                 | 1071.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv0929          | 3.04            | 0.0257          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1036028.103 |
|                 |                 |                 | 7002.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2535c         | 3.95            | 0.0257          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2859300.286 |
|                 |                 |                 | 0355.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2937          | 2.42            | 0.0257          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3273299.327 |
|                 |                 |                 | 4075.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3500c         | -3.9            | 0.0257          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3919220.392 |
|                 |                 |                 | 0062.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv0111          | 1.61            | 0.0352          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.133992.1360 |
|                 |                 |                 | 07.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0820          | 2.45            | 0.0352          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.912726.9135 |
|                 |                 |                 | 02.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv3502c         | -7              | 0.0352          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=PATRIC.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3921087.392 |
|                 |                 |                 | 2040.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </div>
