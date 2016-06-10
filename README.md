## Synopsis

THREDDS Explorer is a QGIS-based plug-in designed to make it easy for users to access georeferenced data accessible through any THREDDS based server.  

Data catalogues and maps are exposed to the user through a simple user interface, which allows him to choose any map or explore all contents of the server without resorting to exploring the default web based THREDDS interface.

This plug-in should work with most THREDDS servers, and will be able to retrieve any layer provided through WMS, WMS-T and/or WCS services published by the server.

[![THREDDS Explorer](https://raw.githubusercontent.com/IHCantabria/THREDDSExplorer/master/doc/video.jpg)](https://vimeo.com/167414368)

## Installation

**Dependencies:** THREDDSExplorer requires the *processing* plug-in by V. Olaya, available within the standard QGIS Installation (also at https://plugins.qgis.org/plugins/processing/).

Installing the plug-in basically involves copying the code in a QGIS "plugins" directory, as detailed below.

Please note that it is mandatory that the folder where the code resides is called "THREDDSExplorer". If you download the code in ZIP format the default name ("THREDDSExplorer-$VERSION") must be changed to "THREDDSExplorer".

### For Windows

The folder where the code should be copied is the following, substituting "`%USERNAME%`" with your user name:

    C:\Users\%USERNAME%\.qgis2\python\plugins

If you want to install the plug-in for all the users in the system, you should use the following folder instead:

    C:\Program Files\QGIS\python\plugins

### For Linux

This procedure has been tested and works on Linux Mint 17.3 and Ubuntu 16.04 LTS, with QGIS 2.14 Essen. It is recommended that you download the latest tagged version (v1.1), via either git or a ZIP file. If you want to get the code in ZIP format:

    $ mkdir ~/.qgis2/python/plugins
    $ cd ~/.qgis2/python/plugins/
    $ wget https://github.com/IHCantabria/THREDDSExplorer/archive/v1.1.zip
    $ unzip THREDDSExplorer-1.1.zip
    $ mv THREDDSExplorer-1.1 THREDDSExplorer
    $ rm THREDDSExplorer-v1.1.zip

If you want to download the code via git:

    $ mkdir ~/.qgis2/python/plugins
    $ cd ~/.qgis2/python/plugins/
    $ git clone https://github.com/IHCantabria/THREDDSExplorer.git
    $ git checkout -b v1.1

The last step (the checkout) will make the v1.1 tag active. If you skip it you will have whatever is the latest code in the repository, instead of a tagged version (not recommended).

If you want to install the plug-in system-wide (for all the users), you can substitute the directory in the examples above with `/share/qgis/python/plugins/`. In that case, you will have to use sudo or be root to `mkdir` the plugins folder, and download content to it.

### For Mac OS X

Installation on OS X has not been tested. Instead, the instructions at qgis.org have been followed (http://docs.qgis.org/1.8/en/docs/user_manual/plugins/plugins.html):

    /Contents/MacOS/share/qgis/python/plugins
    /Users/$USERNAME/.qgis/python/plugins

**NOTES**

* It is possible to define additional paths for QGIS to look for your plug-ins, by defining the `_QGIS_PLUGINPATH_` environment variable with a full path to the new desired plug-in folder.

## User Manual

For more information you can find a PDF manual under the "doc" folder.
