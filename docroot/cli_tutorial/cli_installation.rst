.. _cli-installation:

==============================================
 Installing the PATRIC Command Line Interface
==============================================

The PATRIC project supports the PATRIC command line on the following systems:

 * Apple computers running macOS version 10.11 (El Capitan) or newer. 

 * PCs running Ubuntu Linux version 14 or newer.

 * PCs running Debian Linux or other Linux distributions derived from Debian (e.g. Mint).

 * PCs running Windows 7 or newer. 

Distribution packages for the releases may be found at the `PATRIC github release site 
<https://github.com/PATRIC3/PATRIC-distribution/releases>`_. 

The installation details differ between the major operating systems. We will discuss each in turn.

Installation on macOS
=====================

The macOS version of the PATRIC command line interface is distributed
as a disk image file. The current release is named
``PATRIC-1.018.dmg`` and may be found on the the github release site
`here
<https://github.com/PATRIC3/PATRIC-distribution/releases/tag/1.018>`_.

Download the release disk image file by clicking on `this link to the file
<https://github.com/PATRIC3/PATRIC-distribution/releases/download/1.018/PATRIC-1.018.dmg>`_. Your
browser will begin the download and save the file to your downloads
directory.

If you are using Safari, the download may be found by clicking on the
download stauts icon near the top right of window, or by going to the
View menu and clicking "Show Downloads.

|safari_download_image|

If you are using Google Chrome, the downloaded file will appear in an icon
at the bottom of the Chrome window:

|chrome_download_image|

If you are using Firefox, you will first be prompted to download the
binary file:

|firefox_download_image|

Select "Save File". The file download status will appear in the top right of
the window; click on the download icon to view the status and to open
the downloaded document:

|firefox_download_image_2|

When the download is complete (depending on your internet speed it may
take several minutes since the disk image is 200 megabytes
in size), open the image by clicking on the downloaded file
``PATRIC-1.018.dmg``. 

The disk image will open and the following window will appear:

|mac_disk_image|

To install the distribution, drag the PATRIC icon onto the
Applications icon. This will copy the PATRIC distribution into the
Applications folder on your computer. 

|mac_install_copy_dialog|

If you already an installation
of the PATRIC toolkit on your computer you will see the following
dialog:

|mac_overwrite_installation|

Select "Replace" to replace your existing installation with the
new one. 

To use the PATRIC toolkit, navigate to the Applications folder and
doubleclick on the PATRIC
icon. You should see the following Terminal window appear:

|mac_cli_window|

Installation on Debian / Ubuntu / Mint Linux
============================================

The version of the PATRIC command line interface packaged for Debian
Linu and its derivative distributions (Ubuntu, Mint, etc) is provided
as a Debian ``.deb`` distribution file. The current release is named
``patric-cli-1.018.deb`` and may be found on the the github release site
`here
<https://github.com/PATRIC3/PATRIC-distribution/releases/tag/1.018>`_.

There are several options for installation. The simplest is to
download the installer using a command line tool, and install with
``dpkg``. This method requires a followup call to ``apt-get`` to
resolve dependencies::

  curl -O -L https://github.com/PATRIC3/PATRIC-distribution/releases/download/1.018/patric-cli-1.018.deb
  sudo dpkg -i patric-cli-1.018.deb
  sudo sudo apt-get -f install

It may be simpler to install using the ``gdebi`` tool as it handles
dependency management itself. Ubuntu does not have ``gdebi`` installed
by default so you will need to install it first::

  sudo apt-get install gdebi-core

Then to install with gdebi::

   sudo gdebi patric-cli-1.018.deb

When the install has completed, the PATRIC command line tools will be
available for you to use. They are installed in the system binary
directory ``/usr/bin`` which is accessible in your default
environment.

Installation on Windows
=======================

The macOS version of the PATRIC command line interface is distributed
as a Windows installation package. The current release is named
``PATRIC-1.018.exe`` and may be found on the the github release site
`here
<https://github.com/PATRIC3/PATRIC-distribution/releases/tag/1.018>`_.

Download the release disk image file by clicking on `this link to the file
<https://github.com/PATRIC3/PATRIC-distribution/releases/download/1.018/PATRIC-1.018.exe>`_. Your
browser will begin the download and save the file to your downloads
directory.

Start the installer by doubleclicking the downloaded file. This will
start the installation process. You should be able to take the
defaults for all of the options.

When the installation has completed, you may start a PATRIC command
line window by going to the Start Menu, select All Programs, and then
PATRIC.

.. |safari_download_image| image:: images/safari_download_image.png
.. |chrome_download_image| image:: images/chrome_download_image.png
.. |firefox_download_image| image:: images/firefox_download_image.png
.. |firefox_download_image_2| image:: images/firefox_download_image_2.png
.. |mac_disk_image| image:: images/mac_disk_image.png
.. |mac_install_copy_dialog| image:: images/mac_install_copy_dialog.png
.. |mac_overwrite_installation| image:: images/mac_overwrite_installation.png
.. |mac_cli_window| image:: images/mac_cli_window.png
