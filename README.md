bikedirect-adelaide-web-map
===========================

Bicycle Map Adelaide for website based on OpenStreetMap and DPTI bikedirect data

Techniques used
===============
* Use JOSM as GIS editor with OpenData plugin to import shapefiles
* Use DPTI BikeDirect data, onroad and offroad layers
* Using JOSM select and delete all lines which are "Main Road" to remove
* Using JOSM simplify the ways to 3m accuracy (default)
* Save as geoJSON which renders faster in OpenLayers
* Remove all attributes and merge onroad and offroad layers to reduce file size
* OpenLayers is used to display the map

Issues
======
* Doesn't load in mobile - suggest change to mobile openlayers
* Slow to load - profiling shows it is in drawing the vectors of the bike path layer, suggest combine small segments with larger to reduce number of items to be drawn, alternatively don't display bike layer until zoomed in