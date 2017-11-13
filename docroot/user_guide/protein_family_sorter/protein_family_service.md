# Protein Family Sorter

## Overview
The Protein Family Sorter tool enables researchers to examine the distribution
of specific protein families, known as FIGfams, across different genomes.

## Select Family Type

### FAMILY TYPE

### PATRIC genus-specific families(PLfams):
The genus-specific protein families are computed using only proteins
within a genus and more stringent criteria (MCL inflation = 3.0). This
provides higher sequence similarity and better specificity while
performing within-genus/species or close strain comparisons.

### PATRIC cross-genus families(PGfams):
The cross-genera protein families are computed by clustering
representative proteins from the genus-specific families with slightly
relaxed criteria (MCL inflation = 1.1). This allows cross-genera or
distant homologs to cluster together, which is necessary to support
cross-genera comparative analysis across all microbial genomes.

### FIGFams:
FIGfams are sets of isofunctional homologs, i.e. set of rotein sequences
that are similar along their full length and believed to implement the
same function. FIGfams are derived from a collection of functional
subsystems, as well as correspondences between genes in closely related
strains.
