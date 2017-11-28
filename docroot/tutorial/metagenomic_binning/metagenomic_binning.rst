==============================================
 Using the PATRIC Metagenomic Binning Service
==============================================

Basic Steps
===========

1. Log in to the Patric web site with your Patric credentials.

2. Provide an input file.

3. Open the Binning Service

4. Run Binning

5. Examine Output

Log in to the PATRIC Website
----------------------------

See `website-login <http://docs.patric.local/user_guides/registration.html?highlight=website%20login#login>`__ for information on logging in to the PATRIC website.
You should see something like this:

.. image:: images/website.png

Provide an input file
---------------------

Input to the Binning Service must be found in a PATRIC workspace. You
can upload files or use pre-existing files in your Workspace or found
in other Workspaces available to you. See these tutorials for using
the PATRIC Workspaces (url). You can supply paired reads for assembly,
or you can supply assembled contigs.

Open the Binning Service
------------------------

The binning service is found under Services. Click on services and
find Binning Service in the dropdown. Click on that and you will see
the Binning Service page, like this:

.. image:: images/service-page-1.png

For these tutorial purposes, we will assume you are using a set of
contigs found in a public workspace. 

Start by clicking the folder symbol next to the contigs box. This will
open a Workspace browser.

Click on the Workspaces dropdown and choose Public Workspaces.

.. image:: images/service-page-2.png

You will see a number of public workspaces. Choose the “Binning”
workspace by clicking on the icon to the left of the name Binning.

.. image:: images/service-page-3.png

Choose the Data folder

.. image:: images/service-page-4.png

And finally, choose the dataset ``SRR2188006.contig.fasta``.
This will then take you back to the Binning Service start page.

.. image:: images/service-page-5.png

.. image:: images/service-page-6.png

Next, choose an output folder by clicking on the folder icon next the
OUTPUT FOLDER choice. This will take you to the workspace browser
where you should choose whatever Workspace folder you like. In this
case, we have already created a folder named BinningExperiments, and
we will select it and click on OK.

.. image:: images/service-page-7.png

This will return you to the Binning Service start page where you will
fill in the output file name and genome group name you want for this
run. We chose ``SRR2188006-1`` for both. These are the names of the
respective folders where you will find the result of the Binning run.

.. image:: images/service-page-8.png

Click Submit and your job will start. To check on the progress of the
job, click on the Jobs icon in the lower right of your browser window:

.. image:: images/service-page-8a.png

.. image:: images/service-page-9.png

The binning job will start annotation jobs, as you can see in the
above screenshot. The run we made previously today was job SRR218806
and spawned two annotation jobs. When all the spawned jobs are
complete, the Binning Service run is complete. Refresh your page to
see the updated status in the right-side panel.
