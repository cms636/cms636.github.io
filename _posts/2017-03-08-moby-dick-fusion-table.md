---
layout: post
published: true
category: updates
title: Moby Dick Fusion Table
author: Thatcher
tags: ''
---
<iframe width="500" height="300" scrolling="no" frameborder="no" src="https://fusiontables.google.com/embedviz?q=select+col6+from+1I1A2y69cZWtm3mkhJOmxRUtwVt456AtzTR9JBsWi&amp;viz=MAP&amp;h=false&amp;lat=34.16087835124493&amp;lng=-57.9007177438736&amp;t=1&amp;z=2&amp;l=col6&amp;y=3&amp;tmplt=3&amp;hml=TWO_COL_LAT_LNG"></iframe>

([link](https://fusiontables.google.com/data?docid=1I1A2y69cZWtm3mkhJOmxRUtwVt456AtzTR9JBsWi#map:id=6) in case the embed above doesn't work)

I found Google Fusion Tables to be a rather limiting tool. On the one hand it handles a large amount of data well. Other similar web apps I've used in the past become very slow when dealing with datasets of locations numbering over one thousand. On the other, Fusion Tables offers little in terms of customization. 

Other programs, like CartoDB offer many different map types. Besides the feature map and heat map that FusionTables offers, CartoDB offers clustering-type maps with a variety of visual differences as well as the ability to filter through time. In this case, for example, it would be nice to have a slider to select a certain range of pages or sequences in the book and show just the locations referenced in that range. Fusion Tables does not offer that as an option while CartoDB does. 

Fusion Tables also fails to let you interact much with data besides just location. There is an option to change what image is placed on each location based on a binning mechanism (which I used in my project above), but you are limited to ten bins and you can only change the color and shape of the feature markers. CartoDB exposes a full PostgreSQL query interface that allows the user to make complex relations between any and all fields in the spreadsheet and the different parameters (size, shape, color) of feature markers. I like having the ability to define these kinds of relationships because they allow me to show more information. In Fusion Tables, I have to click each feature to see its exact page, while in CartoDB I could set the color of each marker to be in some way proportional to its page number. Alternatively, I could place bigger markers on the locations that are featured heavily in the book, like Nantucket, by counting the occurence of each location using a SQL query. 

I think CartoDB is a much more powerful option for this project.
