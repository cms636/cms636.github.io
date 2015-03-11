---
layout: post
published: true
title: Coloring the Map
category: updates
author: Meghana Bhat
---

My refined map:
http://cdb.io/1E4K2We
I brought the data set into CartoDB and added a gradient of colors that varies based on page number of the location mention. As you can see in the map, many locations are scattered in terms of page numbers and mentions. However, you can see a bit of a pattern in the way that the locations seem to approach two main locations as the book progresses: the Northeast coast of the US as well as the UK. There is also a shift to talk of the more nothern parts of Asia later in the book. I haven't actually read the book, so I can't make too many conclusions about the reasons for all these mentions and patterns just from looking at this map. However, I think it is worth looking at these patterns.

What I could not implement: It'd help more to be able to see, on the side, the entire page text in which a location was mentioned, perhaps at a click. Right now a hover brings up a little information like page and line and quote, but the quotes are so short they hardly tell anything. Also, some points share sentences--it might be nice to see that relation visualized, such as in the form of a line between the points. It might also be cool to see a sequence of arrows between points around the same area and close page numbers--it might help track paths through the story. Filtering for page number intervals and chapters would also help narrow down on certain groups of mentions--like in Harihar's map. 

I spent a long time trying to get fusion tables to display the color so I could incorporate it as an overlay, but in the end, it refused to accept any notion of styling, so I switched to CartoDB. This, however, meant I did not know how to include the whaling map overlay.
