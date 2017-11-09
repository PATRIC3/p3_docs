===================================
 Developing PATRIC Code at Argonne
===================================

This is a quick guide for PATRIC developers working on the internal
systems at Argonne National Laboratory.

Access
======

One must have a Unix login account at Argonne to be able to develop
in the PATRIC environment. Contact one of the PATRIC staff to get this
if you believe you should be working there.

To get to the internal systems where the PATRIC environment runs one
must first log in to the bastion host ``login.mcs.anl.gov``. From
there the internal machines are visible. A useful machine to use is
``holly.mcs.anl.gov``.

Environment
===========

The PATRIC code deployments are in two parts. A *runtime library*
incorporates all the basic software required to run the
PATRIC-specific code (language interpreters and associated runtime
libraries; bioinformatic analysis tools; libraries and development
tools that do not come with the base OS; etc).

The *deployment* contains all the PATRIC-specific code that typically
changes much more often and is part of the PATRIC release cycle.

On the Argonne machines, the runtime library is typically located on
local disk on the machines that run PATRIC components in the path
``/disks/patric-common/runtime``. 

On the Argonne systems that have PATRIC deployments installed, the
standard deployment location is ``/disks/p3/deployment``. The software
deployment infrastructure creates user environment configuration
scripts to set up the environment for the execution of the PATRIC
scripts and the associated runtime routines. These may be sourced in
your environment via the command::

  source /disks/p3/deployment/user-env.sh

Testing Existing Applications
=============================

One of the common uses for using raw access to the Argonne systems is
the testing of service backends without going through the job
submission infrastructure. To do this one must understand a little
about how the application service works.

Each application is defined by an application specification
document. This document specifies the inputs that the service
expectes. For example, the phylogenetic tree application assumes the
following configuration::

   {
     "script": "App-PhylogeneticTree",
     "label": "Compute phylogenetic tree",
     "id": "PhylogeneticTree",
     "description": "Computes a phylogenetic tree given a set of in-group and out-group genomes",
     "parameters": [
       {
         "required": 1,
         "desc": "Path to which the output will be written. ",
         "type": "folder",
         "default": null,
         "label": "Output Folder",
         "id": "output_path"
       },
       {
         "required": 1,
         "desc": "Basename for the generated output files.",
         "type": "wsid",
         "default": null,
         "label": "File Basename",
         "id": "output_file"
       },
       {
         "id": "in_genome_ids",
         "label": "In-group genomes",
         "allow_multiple": true,
         "required": 1,
         "type": "list",
         "default": []
       },
       {
         "id": "out_genome_ids",
         "label": "Out-group genomes",
         "allow_multiple": true,
         "required": 1,
         "type": "list",
         "default": []
       },
       {
         "id": "full_tree_method",
         "required": 0,
         "default": "ml",
         "label": "Full tree method",
         "desc": "Full tree method",
         "type": "string"
       },
       {
         "id": "refinement",
         "required": 0,
         "default": "yes",
         "label": "Automated progressive refinement",
         "desc": "Automated progressive refinement",
         "type": "string"
       }
     ]
   }

The application specifications may be found in the `app_service repository at
github <https://github.com/TheSEED/app_service/tree/master/app_specs>`_. 

Each application service is implemented by a program named
``App-ApplicationName``. Thus the phylogenetic tree application is
called ``App-PhylogeneticTree``. Sources for the applications are
also found in the `app_service repository at
github <https://github.com/TheSEED/app_service/tree/master/scripts>`_. 

All of the application scripts accept the same parameters, described
by its usage statement::

 $ App-PhylogeneticTree -h
  Usage: /disks/p3/deployment/plbin/App-PhylogeneticTree.pl app-service-url app-definition.json param-values.json [stdout-file stderr-file]

The ``app-definition.json`` parameter is the application specification
document mentioned above. The ``param-values.json`` parameter is
another JSON file that defines the actual values of the parameters as
defined in the specification document.

An example of a parameters file for the phylogenetic tree application
is the following::

    $ cat tree.in
    {
       "in_genome_ids": [
           "66976.18",
           "1262772.3",
           "1262773.3"
       ],
       "out_genome_ids": [
           "66976.17"
       ],
       "output_path": "/olson@patricbrc.org/test",
       "output_file": "tree-15",
       "full_tree_method": "ft",
       "refinement": "no"
    }

Here, we request a phylogentic tree with three in-group genomes and
one out-group genome, with the output to be written to the folder
``/olson@patricbrc.org/test`` in the PATRIC workspace with the output
name to be ``tree-15``. The full tree method request is FastTree, and
no refinement is requested.

We may run this application as follows. We give the application script
a bogus first parameter; in production execution that is a URL that
will result in the standard output and error streams to be fed in
realtime to the application service where it is logged and available
for display in the PATRIC website.

::

    $ App-PhylogeneticTree xx /disks/p3/deployment/services/app_service/app_specs/PhylogeneticTree.json tree.in
    Process tree $VAR1 = {
              'parameters' => [
                                {
                                  'id' => 'output_path',
                                  'type' => 'folder',
                                  'desc' => 'Path to which the output will
    			      be written. ',
                                  'default' => undef,
                                  'required' => 1,
                                  'label' => 'Output Folder'
                                },
    [....]

We see the execution beginning here. There is a fairly large amount of
debugging output from both the application service infrastructure as
well as the tools invoked by the application service infrastructure to
accomplish the computation desired.
