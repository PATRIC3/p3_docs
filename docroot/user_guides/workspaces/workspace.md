# PATRIC Private Workspace

## Overview
The PATRIC Workspace provides a private area in the website for uploading data, running analysis services on the data, storing the analysis results, and managing groups of data created within the PATRIC website.

### See also:
  * [Groups](../groups.html)
  * [Data Upload](../data_upload.html)
  * [Registration](../registration.html)
  * [Services and Tools](../services_tab.html)

## Accessing the Private Workspace on the PATRIC Website
Registration is required to use the PATRIC private Workspace. The registration link is at the top right corner of the PATRIC website. If you have already registered, clicking the Login button beside the registration link will display the Login page. 

![Register and Login Buttons](../images/register_login_buttons.png)

After logging in, the Workspaces option in the top Menu Bar will become populated with the available workspaces for the logged-in user. 

![Workspaces Menu](../images/workspaces_menu.png)

The default workspace is called "home," which is the top level workspace containing all the files, folders, and job results for the logged in user. Additional shared workspaces may also be available (see Shared Workspaces below).

![Home Workspace](../images/workspace_home.png)

The table in the workspace lists the Names of folders and files, their Size (files only), the Owner ("me" unless the file or folder was shared by another user), other Members (users) with whom the workspace is shared, and when the file or folder was Created. Double-clicking a folder opens it and displays the contents. Double-clicking the "Parent Folder" at the top of the list moves back up the folder hierarchy and displays contents of the higher level folder. 

## Workspace Tools
Generally, within the Workspace, you can Upload files, Add Folders, and Show Hidden files and folders. Each of these is described below.

### Upload
See [Data Upload](../data_upload.html) for details.

### Add Folder
Initially, the home Workspace is pre-populated with several folders that correspond to common PATRIC data types and are the default locations for data of those type, listed below. Additional custom folders can be created using the Add Folder button at the top right of the workspace table.

* Experiment Groups
* Experiments
* Feature Groups
* Genome Groups

### Show Hidden
When running jobs in PATRIC, some ancillary files are stored in hidden folders to simplify the display. In most cases, access to these files is not needed. However, in some cases, such as annotating contig files from an assembly job, access to the hidden contig files is needed. The Show Hidden button at the top left of the Workspace table will show the hidden files. Clicking the button again (now labeled "Hide Hidden") will hide the files again.

### Action buttons

After selecting one or more of files or folders in the Workspace, a set of options becomes available in the vertical green Action Bar on the right side of the table.  These include

* **Hide:** Toggles (hides) the right-hand side Details Pane.
* **Download:** Downloads the selected item.
* **Delete:** Deletes the selected items (rows).
* **Rename:** Allows renaming the selected item.
* **Copy:** Creates copies the selected items and allows the copies to be put into another folder in the Workspace.
* **Move:** Allows moving of the selected item(s) into another folder in the Workspace.
* **Edit Type:** Allows changing the data type of the selected item. This will change how the Workspace interprets the item. This feature is generally only used when uploading a new data file into the Workspace.  Options include
  * unspecified (default)
  * contigs
  * nwk (Newick file)
  * reads (sequence)
  * diffexp_input_data (expression data)
  * diffexp_input_metadata (metadata for expression data)
