---
layout: post
published: true
category: updates
title: Melville data visualization idea
author: Tyler
---
I don't have much yet for this, but my idea is to have an interactive map that highlights the most likely places Melville will visit from any location you select.

Here is a very abstract and low-fidelity animation of what it might be like:
![melville-animation.gif]({{site.baseurl}}/assets/melville-animation.gif)

So, instead of just seeing his travels one by one, and since Melville often revisits the same places, it might be interesting to visualize a probability distribution of his travels directly over the map. I'll be implementing this in D3 and have not figured out exactly yet how the probability calculations are going to work...but I think I'll keep it simple and make a basic naive bayes classifier.