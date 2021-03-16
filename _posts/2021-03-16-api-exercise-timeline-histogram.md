---
layout: post
published: true
category: updates
title: API Exercise - Timeline Histogram
author: Trevor Morrisey
tags: ''
---
I decided to do something similar to one of the examples and create a timeline of the objects in the collection. Rather than showing the date for each individual object, I grouped them into centuries and generated a histogram to show how heavily different time periods are represented in the collection. I had planned to have labels appear for each segment of the histogram when hovered but that ended up being difficult to implement. For now, I added permanent text labels next to the histogram instead to make sure that information is available somewhere. Also, in the data returned by the API, the labeling for centuries is inconsistent. From the 20th century BCE up to the 5th century CE, all centuries are labeled as either "BCE" or "CE." However, from the 6th century CE onward, the "CE" is omitted. I chose not to fix this manually in case the formatting in the data is changed later.

[https://editor.p5js.org/TrevorMorrisey/present/O9NoLQWC5](https://editor.p5js.org/TrevorMorrisey/present/O9NoLQWC5)