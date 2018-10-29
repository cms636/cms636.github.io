---
layout: post
published: true
category: updates
title: 'Mapping Space, Time, and Narrative'
author: 'Amy Shim, Yichen Jia, Cindy Liu'
---
In our rough draft, we came up with this model in ArcGIS:
![zoomin (1).PNG]({{site.baseurl}}/assets/zoomin (1).PNG)
Using the point-to-line tool we created a map of Melville's routes as provided in the dataset, darkening the lines as his journey grew later in time. Through the use of a color gradient, we introduced a third axis, time, into a two-dimensional map.

This graph is limited in that we used straight lines to connect two locations. We did not follow real urban configurations, as Wyn Kelley did in her maps. That would be complicated as you would have to insert a historical map of London into the ArcGIS software and use graph algorithms (or even more labor-intensive, hand-draw) the routes he might have taken by following existing streets and walkways.

However, we did manage to come up with another interesting visualization. Using the kernel tool, we generated a heat map showing the areas Melville most frequented. This was rather difficult as he went to some bizarre, out of the way locations occasionally, as you can see in a zoomed out version of the gradient map.

![]({{site.baseurl}}/assets/zoomedout.PNG)
![kernel.PNG]({{site.baseurl}}/assets/kernel.PNG)

The heat map shows us three main areas of London most frequented by Melville. Most obvious, Melville spent the most time around his neighborhood in Craven Street, where he lived for the two months in 1849 detailed in the journal we are drawing our data from. We also see that he spent much time in the Mayfair neighborhood, an affluent area of London (at the time and now) with many businesses, shops, and churches. He also spent time in the Temple, one of the main historic legal districts of England, and Ludgate Hill.

