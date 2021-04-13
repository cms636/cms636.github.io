---
layout: post
published: true
category: updates
title: AR.js Exercise
author: Delace Jia
---
For me, this exercise was a little easier than the API exercise because there was less processing of raw data and less UI development. I created my own markers, and found that some of them worked better than others (and had to scrap almost all of them because they wouldn’t work, mostly ones with low-quality patterns / light borders). I also was having a hard time using the Glitch interface and referencing assets, and it took a while to realize that Glitch was a platform for instantaneous site editing and not something used specifically for AR. I ended up looking up Jasmine’s starter code on Github and instead made a Github Pages instead of a Glitch page. 

I have the standard Hiro marker that brings up some text as well as a pattern of fish I made a while back. My other marker is a personally made pattern with an image of string lights inside. It shows a cylinder when in view. I found some code online that plays audio whenever a 3D shape is present, and I used it to play a song whenever the cylinder is in view. The script for it uses JavaScript, and while I can understand generally what it does, I’m still very unused to the JavaScript syntax and the use of components. On the AR.js documentation, they also note that audio requires a user interaction on iOS (like a click), so the script I use doesn’t work on the phone (it does work when I use my webcam on my laptop). I’ve attached some of my custom markers below (only the string light one works, sadly), and an image of the website displaying the components over them. The link to my site is here: https://delacejia.github.io/AR-practice/A-frame/ 

![manymarkers.png]({{site.baseurl}}/assets/manymarkers.png)
![ar_exercise.jpg]({{site.baseurl}}/assets/ar_exercise.jpg)
