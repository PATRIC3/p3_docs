
.. _cli::p3-get-family-features:

######################
p3-get-family-features
######################

.. highlight:: perl


.. _cli::Return-Features-From-Families-in-PATRIC:

***************************************
Return Features From Families in PATRIC
***************************************



.. code-block:: perl

     p3-get-family-features [options]


This script returns data for all the features in one or more protein families from the PATRIC database. It supports standard filtering
parameters and the specification of additional columns if desired. In addition, the results can be filtered by genomes
from a secondary input file. As currently coded, the command may fail if the number of genomes in the secondary file is
large.

.. _cli::Parameters:

Parameters
==========


There are no positional parameters.

The standard input can be overridden using the options in :ref:`cli-input-options`.

Additional command-line options are those given in :ref:`cli-data-options` and :ref:`cli-column-options` plus the following.


gFile
 
 Name of a tab-delimited file containing genome IDs. If specified, only features in these genomes will be returned.
 


gCol
 
 Index (1-based) or header name of the column containing the genome IDs in the genome file. The default is
 \ ``genome.genome_id``\ .
 


ftype
 
 The type of family being used. The default is \ ``local``\ , indicating PATRIC local protein families. Other options are
 \ ``figfam``\  or \ ``global``\ .
 


fields
 
 List the available field names.
 



