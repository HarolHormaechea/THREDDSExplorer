**CURRENT**

* Utilities.py
    - Added function to check platform (Windows vs Linux)


* WCSParser.py
    - Create temporal file to store the .tiff from the WCS request for one point
    in time

**v1.1** (2016-06-10)

* ServerDataPersistenceManager.py
    - Solved bug when reading variable "GDALVersionErrorSetting" (2016.06.06)


* Visor_UI.py
    - Moved GDAL version warning to WCS tab for Linux users


* ServerDataPersistenceManager.py
    - Do not show server list window on `__init__` method


* VisorController.py
    - Show server list window when button is clicked


* THREDDS_Explorer_dockwidget_base.ui, THREDDS_Explorer_dockwidget.py
    - Add vertical and horizontal scrolls to the plugin's main user interface


* General
  - Trace errors into QGIS/THREDDSExplorer registry tab
  - ui2py: script to automate .ui to .py conversion (2016-06-10)

**v1.0** (2016-05-31)

* Connect to THREDDS Server
* List THREDDS Server contents
* Download WMS
* Download WCS
* Animate WMS/WCS layers
