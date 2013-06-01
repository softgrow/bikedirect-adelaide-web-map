bikedirect-adelaide-web-map
===========================

Bicycle Map Adelaide for website based on OpenStreetMap and DPTI bikedirect data

Techniques used
===============
* Use JOSM as GIS editor with OpenData plugin to import shapefiles
* Use DPTI BikeDirect data, onroad and offroad layers
* Using JOSM select and delete all lines which are "Main Road" to remove
* Save as JeoJSON which renders faster in OpenLayers
* OpenLayers is used to display the map
