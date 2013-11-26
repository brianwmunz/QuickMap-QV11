quickMap-QV11
==============

A combination of my old qlikMap extension (http://market.qlikview.com/qlikview-qlik-map.html) and the kml map extension(http://community.qlikview.com/thread/45125?tstart=0).

This extension will not initially load with the coordinate data dimension in case only the KML functionality is needed.  To add the coordinate dimension, click the (+) in the dimension section at the top of the properties panel.

Please see the qvw for info on how to set up the dimension for coordinates if plotting them with your data.

In order to use your own kml, the extension of the kml needs to be changed from .kml to .xml.  For example, countries.kml needs to be changed to countries.xml.  Then simply place it in the quickMap extension folder and set the property to the filename

*********************************
      DISCLAIMER/WARNING       
*********************************
There are a million types of KMLs out there of various quality.  This extension does its best to read shapes from KML files.  If yours isn't loading, check to make sure the KML shape IDs match your region dimension.

ALSO, KML files can be very large.  This extension in general is meant for a small amount of map data since it uses only front-end client-side technology.  The most useful thing the KML reading could be used for is if you have a need for custom regions that are proprietary to you, for example sales territories.  You could easily draw out a KML of these territories and load them in, assuming, again, the KML file isn't too large.

For larger amounts of data, some sort of server side solution is needed.  That being said, you could always split up a giant KML into smaller sections and have them load dynamically.  



