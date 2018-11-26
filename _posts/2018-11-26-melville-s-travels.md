---
layout: post
published: true
category: updates
title: Melville's Travels
author: Abnell Comas
---
For this project, I used the MapBox API to geo-reference the Melville in London data to a 1849 London Map and a contemporary one(unfortunately was not able to find a free one on Open Street Map so I used a cartoonish one I found on MapWarper, which still illustrates the point). The purpose of this project is to allow users to compare locations Melville was at in 1849 vs where would those locations be now. 

The project allows user to move around the map and see data points, change the underlying map layer, and click on data points to see more info regarding that data point. 

Below you can see a example picture of how a section of the map may look with the 1849 map.

![points1849.PNG]({{site.baseurl}}/assets/points1849.PNG)

Then if you hover over the controls on the top right corner you can change the map to be a contemporary one, which would look nicer with a better map but this one will have to do.

![pointsNow.PNG]({{site.baseurl}}/assets/pointsNow.PNG)

You can also click on points to get a popup with data from that point. 

![popup.PNG]({{site.baseurl}}/assets/popup.PNG)


This project required to have map tiles, a tool such as GeoJson.io that can convert excel spreadsheets to a list of feature data points(can be done by yourself since all its doing is formatting it into a json object), the MapBox API, and some javascript,html, and css coding to put it all together. 

In terms of limitations of the tools, GeoJson.io had the problem that only 185 spreadsheet data rows may be added at a time, so I had to manually divide the points into 4 files containing 100 points and then adding them. Also it had problems with data points containing no coordinates, so those had to be removed as well, and if coordinates were formatted weirdly(for example some of the data coordinates contained extra commas) it would not accept them either and give you no error message, just no response from the map or the constructed json. Finally, not having access to decent map tiles can make the project complicated since one may end up having to construct their own. 
