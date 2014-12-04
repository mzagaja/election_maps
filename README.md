election_maps
=============

Right now I am working on creating election maps for the state of Connecticut using D3JS. My goal is to learn how to use
geographic functions in D3JS and also make some useful town by town election maps that can be incorproated into websites.

The town by town map was downloaded from http://magic.lib.uconn.edu/connecticut_data.html from the [2010 
Redistricting Census Data](http://magic.lib.uconn.edu/magic_2/vector/37800/townct_37800_0000_2010_s100_census_1_shp.zip). I then converted it to GeoJSON using ogr2ogr and then topoJSON. 

I am following the tutorial at http://bost.ocks.org/mike/map/ and adopting it for my Connecticut map. You can see the iterations of my work in the pltownct_37800_0000_2010_s100_census_1_shp/wgs84 subfolder. You may find the HTML file variations useful in debugging or analyzing your own map making process. Connecticut 2.json, 20, and 80 are all files that have been run through [Mapshaper](http://mapshaper.org) to reduce the JSON file size and increase load time. You can use them to see the impact of using Mapshaper to do this. You will likely notice a slow load time with the JSON file I decided to stick with in the end. This can be reduced if it is gzipped or placed on a server that automatically GZIPs files.

One pitfall was figuring out how to project the map. I used mostly trial and error after downloading Bostock's
http://bl.ocks.org/mbostock/3734308 to more easily position it. The settings in the projection were about equal.

A live copy is available at [http://wnext.net/2008ct/connecticut-test.html](http://wnext.net/2008ct/connecticut-test.html).

The PDF is a copy of the presentation I gave on this map to the [NewHaven.io](http://www.newhaven.io) Civic Hack Night Meetup Group in March.