---
layout: post
published: true
title: "Moby Dick - Making Maps"
category: updates
author: Meridian Witt
---

After missing class, I was worried I would be behind but I am already familiar with the Google Maps API. I was excited to learn about Fusion Tables. I would have loved to use it when I created a map of some [Historically Black Neighborhoods](http://cs.wellesley.edu/~mwitt/cs249/AM3/am3.html) for a class. We used data from a Wikipedia page (we ended up hard coding in the latlongs, although we could have used JSON using Kimono). 

However, I found FusionTable layers to unwieldly (difficult to customize infoWindows, create onClick events). It would have been easier to convert the FusionTable into JSON and recreate from there (or I will work with CartoDB). So, I have a [very simple map](http://cs.wellesley.edu/~mwitt/cs249/DH/FusionTables/fusiontable.html) of the Moby Dick location references. 

My design proposals:
- onClick: make a call to the Wikipedia API for an extract from a page about the location clicked 
- onClick: make a call to the Yelp API to find a nearby cafe to read the book on location
- overlay a map of Herman Meville's travels
- overlay a map of popular travel locations in his time period
- overlap a map of the most mentioned places in the new in his time
- a slider time progression (per chapter intervals) : a good chapter summary



