
.. _cli::p3-file-filter:

##############
p3-file-filter
##############

.. highlight:: perl


.. _cli::Filter-a-File-Against-Contents-of-a-Second-File:

***********************************************
Filter a File Against Contents of a Second File
***********************************************



.. code-block:: perl

     p3-file-filter.pl [options] filterFile filterCol


Filter the standard input using the contents of a file. The output will contain only those rows in the input file whose key value
matches a value from the specified column of the specified filter file. To have the output contain only those rows in the input
file that do NOT match, use the \ ``--reverse``\  option. This is similar to :ref:`cli::p3-merge`, except that script operates on whole
lines instead of a single key field.

.. _cli::Parameters:

Parameters
==========


The positional parameters are the name of the filter file and the index (1-based) or name of the key column in the filter file.
If the latter parameter is absent, the value of the \ ``--col``\  parameter will be used (same name or index as the input file).

The standard input can be overriddn using the options in :ref:`cli-input-options`.

Additional command-line options are those given in :ref:`cli-column-options` plus the following.


reverse
 
 Instead of only keeping input records that match a filter record, only keep records that do NOT match.
 



