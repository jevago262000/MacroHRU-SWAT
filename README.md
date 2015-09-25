# MacroHRU-SWAT

*Macro to average HRU's annual outputs of SWAT*

The macro allows user to average the Hydrological Response Units (HRU’s) results from an annual run of the Soil and Water Assessment Tool ([SWAT](http://swat.tamu.edu/)). The result is a spatially multi-annual average of all the HRU’s for the period selected by the user. Joining the results obtained from the run to the HRU’s shapefile, it is possible to make maps and analyze any variable of the water balance over the basin.

This macro is presented in both languages English and Spanish. It was developed in Visual Basic for Applications (VBA) under ArcGIS platform.

This document is a guide to ensure the correct operation of the macro. This macro works correctly in ArcGIS 9.3. If you will work with ArcGIS 10, you will need to follow the next steps:

#### STEP 1

First of all, it is necessary to have installed VBA on ArcGIS 10. ArcGIS 10 does not have the VBA package installed by default; hence, you must install it as follows:

**To use map documents that contain VBA code for ArcGIS Desktop Concurrent Use** 

The VBA license needs to be authorized on the license manager on your network. You can check if a VBA license is available for use by viewing the Availability list in ArcGIS Administrator after setting the license manager. Contact your organization's license administrator to authorize VBA licenses if you do not have any VBA licenses.

1.	Install ArcGIS Desktop VBA Resources for Developers from the installation media if you haven't done so already.
2.	Open ArcGIS Administrator, click Desktop in the table of contents, and then make sure you have the appropriate concurrent use product selected and the license manager set.

**To use map documents that contain VBA code for ArcGIS Desktop Single Use**

1.	Install ArcGIS Desktop VBA Resources for Developers from the installation media if you haven't done so already.
2.	Open ArcGIS Administrator, click Desktop in the table of contents, then make sure you have the appropriate single use product selected.
3.	Click Authorize Now and follow the instructions to authorize VBA. If you have requested the authorization number for VBA, it would have been in an e-mail from Esri Customer Service. It will also be visible in the Authorization and Provisioning section of the Customer Care site. If you cannot locate this information, contact [Esri Customer Service](https://service.esri.com/index.cfm?fa=homepage.feedback.customer_serviceform).

The previous explanation was taken from [ArcGIS Resource Center](http://help.arcgis.com/en/arcgisdesktop/10.0/help/index.html#//000300000014000000.htm). If you are interested in a more detailed explanation please refer to http://gis.stackexchange.com/questions/15656/install-vba-on-arcgis-10.

#### STEP 2

Open the file *.mxt by double click. This file contains the macro to average the results of HRU’s in an annual run. If you get a warning while opening the macro on ArcGIS 10, please follow these steps:

1.	In the folder attached with this email, you will find the file mscomct2.ocx, which controls dates in VBA. You will need to copy this *.ocx file in these paths:

  a.	C:\Windows\SysWOW64 and
  
  b.	C:\Windows\System32
2.	You will need to register this file using the command line, with the tool regsvr32 (bear in mind you will need administrative privileges) in both folders:

  a.	C:\Windows\SysWOW64>regsvr32 mscomct2.ocx
  
  b.	C:\Windows\System32>regsvr32 mscomct2.ocx

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
