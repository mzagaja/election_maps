election_maps
=============

Right now I am working on creating election maps for the state of Connecticut using D3JS. My goal is to learn how to use
geographic functions in D3JS and also make some useful town by town election maps that can be incorproated into websites.

The town by town map was downloaded from http://magic.lib.uconn.edu/connecticut_data.html#election from the 2010 
Redistricting Census Data. I then converted it to GeoJSON using ogr2ogr and then topoJSON. 

I am following the tutorial at http://bost.ocks.org/mike/map/ and adopting it for my Connecticut map.

One pitfall was figuring out how to project the map. I used mostly trial and error after downloading Bostock's
http://bl.ocks.org/mbostock/3734308 to more easily position it. The settings in the projection were about equal.
