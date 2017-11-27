===================
Flute Experiment 2
===================

Peptidoglycan synthesis in Mycobacterium tuberculosis is organized into networks with varying drug susceptibility
==================================================================================================================

**Publication: PMCID:**
`PMC4620856 <http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4620856/>`__

Peptidoglycan (PG), a complex polymer composed of saccharide chains
crosslinked by short peptides, is a critical component of the bacterial
cell wall. PG synthesis has been extensively studied in model organisms
but remains poorly understood in mycobacteria, a genus that includes the
important human pathogen Mycobacterium tuberculosis (Mtb). The principle
PG synthetic enzymes have similar and, at times, overlapping functions.
To determine how these are functionally organized,we carried out whole
genome transposon mutagenesis screens in Mtb strains deleted for ponA1,
ponA2, and ldtB, major PG synthetic enzymes. We identified distinct
factors required to sustain bacterial growth in the absence of each of
these enzymes. We find that even the homologues PonA1 and PonA2 have
unique sets of genetic interactions, suggesting there are distinct PG
synthesis pathways in Mtb. Either PonA1 or PonA2 is required for growth
of Mtb, but both genetically interact with LdtB, which has its own
distinct genetic network. We further provide evidence that each
interaction network is differentially susceptible to antibiotics.
Thus, Mtb uses alternative pathways to produce PG, each with its own
biochemical characteristics and vulnerabilities.

| Experimenter/researcher/owner of data: Karen Kieser
| PI/lab: Eric Rubin, Harvard School of Public Health
| Uploaded/deposited by: Thomas Ioerger, Texas A&M University
| Publication: manuscript in preparation (K. Kieser et al.)
| Dataset: dPonA1_KOD.wig
| SRA accession: SRA277968
| http://www.ncbi.nlm.nih.gov/sra/?term=SRA277968%5Baccn%5D
| Library: This TnSeq library consists of insertion mutants of
  the Himar1 transposon in a Rv0050/PonA1-deletion mutant of the
| M. tuberculosis H37Rv strain, constructed by Karen Kieser in the Rubin
  lab.
| Conditions: grown on plates with 7H10 medium
| Transposon used: Himar1
| Protocol for library preparation: Himar1 transfection as described
  in Long et al (2015).
| Protocol for TnSeq sample preparation: nested PCR, as described
  in Long et al (2015).
| Protocol for DNA extraction: (perhaps not relevant)
| Protocol for sequencing: 54 bp paired-end reads on Illumina
  GAII (sequencing date: 4/2/2013)
| Protocol for data processing: mapped reads to reference genome using
  TRANSIT (Ioerger et al., 2015);
| Reported as unique template counts at TA dinucleotides
| Reference genome: M. tuberculosis H37Rv (GenBank refseq accession
  number: NC_000962.2)

**References:**

Long, J.E., DeJesus, M., Ward, D., Baker, R.E., Ioerger, T.R. and Sassetti, C.M. (2015). Identifying essential genes in Mycobacterium tuberculosis by global phenotypic profiling. in: Methods in Molecular Biology: Gene Essentiality, (Long Jason Lu, ed.), vol. 1279. DeJesus, M.A., Ambadipudi, C., Baker, R., Sassetti, C., and Ioerger, T.R. (2015). TRANSIT – a Software Tool for Himar1 TnSeq Analysis. PLOS Computational Biology, to appear.

**Results Dataset:** `resampling_dPonA1_wt.xlsx <ftp://ftp.patricbrc.org/BRC_Mirrors/FLUTE/Experiment_2/resampling_dPonA1_wt.xlsx>`_

**Conditional Essentials:**

The following genes are indicated as conditional essentials based
on statistical analysis (resampling) output using Transit software
(http://saclab.tamu.edu/essentiality/transit/). In this method, for each
ORF (e.g., Rv0001) Transit calculates to determine whether the
essentiality of the gene significantly increase or decreases. The
adjusted p-value uses the Benjamini-Hochberg correction for multiple
tests, with a threshold of <0.05 for significance.

**resampling_dPonA1_wt data set**

.. raw:: html

   <div>

+-----------------+-----------------+-----------------+-----------------+
| **ORF**         | **log2 FC**     | **q-value**     | **Feature in    |
|                 |                 |                 | PATRIC**        |
+-----------------+-----------------+-----------------+-----------------+
| Rv0007          | -8.44           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.9914.10828. |
|                 |                 |                 | fwd>`__         |
+-----------------+-----------------+-----------------+-----------------+
| Rv0050          | -9.59           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.53663.55699 |
|                 |                 |                 | .fwd>`__        |
+-----------------+-----------------+-----------------+-----------------+
| Rv0096          | -3.59           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.105324.1067 |
|                 |                 |                 | 15.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0097          | -4.03           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.106734.1076 |
|                 |                 |                 | 03.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0101          | -1.74           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.110001.1175 |
|                 |                 |                 | 39.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0127          | -3.35           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.154232.1555 |
|                 |                 |                 | 99.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0155          | -6.58           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.183622.1847 |
|                 |                 |                 | 22.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0157          | -5.93           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.185052.1864 |
|                 |                 |                 | 79.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0211          | -6.04           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.251782.2536 |
|                 |                 |                 | 02.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0238          | -8.61           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.288428.2890 |
|                 |                 |                 | 42.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0455c         | -5.73           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.545375.5458 |
|                 |                 |                 | 21.rev>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0467          | -6.84           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.557527.5588 |
|                 |                 |                 | 13.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0489          | -5.36           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.578426.5791 |
|                 |                 |                 | 75.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0642c         | -4.97           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.736298.7372 |
|                 |                 |                 | 03.rev>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0643c         | -2.38           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.737268.7381 |
|                 |                 |                 | 49.rev>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0806c         | -7.42           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.899732.9013 |
|                 |                 |                 | 30.rev>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv0860          | -2.83           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.956293.9584 |
|                 |                 |                 | 55.fwd>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv1086          | -7.96           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1210595.121 |
|                 |                 |                 | 1383.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1112          | -4.18           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1238255.123 |
|                 |                 |                 | 9328.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1339          | -4.55           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1505917.150 |
|                 |                 |                 | 6738.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1421          | -2.29           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1595979.159 |
|                 |                 |                 | 6884.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1565c         | -5.85           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1771640.177 |
|                 |                 |                 | 3829.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1798          | -3.72           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2036700.203 |
|                 |                 |                 | 8532.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1836c         | -2.57           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2082603.208 |
|                 |                 |                 | 4636.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2140c         | -5.52           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2399798.240 |
|                 |                 |                 | 0328.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2171          | -8.78           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2432951.243 |
|                 |                 |                 | 3634.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2176          | -3.78           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2437941.243 |
|                 |                 |                 | 9140.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2222c         | -1.95           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2492402.249 |
|                 |                 |                 | 3742.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2224c         | -3.49           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2495461.249 |
|                 |                 |                 | 7023.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2404c         | -5.02           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2701287.270 |
|                 |                 |                 | 3248.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2535c         | -4.47           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2859300.286 |
|                 |                 |                 | 0418.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2864c         | -2.86           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3175454.317 |
|                 |                 |                 | 7265.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3302c         | 10.81           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3687685.368 |
|                 |                 |                 | 9442.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3484          | -1.96           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3903078.390 |
|                 |                 |                 | 4616.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3490          | -4.67           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3908236.390 |
|                 |                 |                 | 9738.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3682          | -8.89           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.4121916.412 |
|                 |                 |                 | 4348.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3910          | -4.88           | 0               | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.4396597.440 |
|                 |                 |                 | 0151.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv0066c         | -3.32           | 0.0095          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.72274.74511 |
|                 |                 |                 | .rev>`__        |
+-----------------+-----------------+-----------------+-----------------+
| Rv0153c         | -4.02           | 0.0095          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.181155.1819 |
|                 |                 |                 | 85.rev>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv1410c         | -2.08           | 0.0095          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1586210.158 |
|                 |                 |                 | 7766.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1432          | -3.7            | 0.0095          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1609849.161 |
|                 |                 |                 | 1270.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1780          | -1.98           | 0.0095          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2014699.201 |
|                 |                 |                 | 5262.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1248c         | -3.79           | 0.017           | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1389357.139 |
|                 |                 |                 | 3052.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1371          | -3.3            | 0.017           | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1543359.154 |
|                 |                 |                 | 4828.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2038c         | -3.26           | 0.017           | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2283723.228 |
|                 |                 |                 | 4796.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2940c         | -1.08           | 0.017           | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3276380.328 |
|                 |                 |                 | 2715.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3529c         | -2.95           | 0.017           | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3965884.396 |
|                 |                 |                 | 7038.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1662          | -2.85           | 0.0249          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1881704.188 |
|                 |                 |                 | 6512.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv0180c         | 8.32            | 0.0307          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.210892.2122 |
|                 |                 |                 | 50.rev>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv1183          | -1.54           | 0.0307          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1321520.132 |
|                 |                 |                 | 4528.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2246          | -4.65           | 0.0307          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2519396.252 |
|                 |                 |                 | 0712.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv3210c         | -4.47           | 0.0307          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3586844.358 |
|                 |                 |                 | 7539.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1401          | -2.81           | 0.0369          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1576930.157 |
|                 |                 |                 | 7532.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2462c         | -1.79           | 0.0369          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2763891.276 |
|                 |                 |                 | 5291.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv0260c         | -2.99           | 0.0413          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.311514.3126 |
|                 |                 |                 | 59.rev>`__      |
+-----------------+-----------------+-----------------+-----------------+
| Rv1220c         | -3.27           | 0.0413          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.1363503.136 |
|                 |                 |                 | 4150.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv1791          | -7.46           | 0.0413          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2029904.203 |
|                 |                 |                 | 0203.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2809          | -3.36           | 0.0413          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.3115408.311 |
|                 |                 |                 | 5719.fwd>`__    |
+-----------------+-----------------+-----------------+-----------------+
| Rv2131c         | -3.93           | 0.0473          | `Feature        |
|                 |                 |                 | page <https://w |
|                 |                 |                 | ww.patricbrc.or |
|                 |                 |                 | g/portal/portal |
|                 |                 |                 | /patric/Feature |
|                 |                 |                 | ?cType=feature& |
|                 |                 |                 | cId=RefSeq.8333 |
|                 |                 |                 | 2.12.NC_000962. |
|                 |                 |                 | CDS.2392517.239 |
|                 |                 |                 | 3320.rev>`__    |
+-----------------+-----------------+-----------------+-----------------+

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </div>
