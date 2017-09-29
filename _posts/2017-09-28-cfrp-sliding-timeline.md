---
layout: post
published: true
category: updates
title: CFRP Sliding Timeline
author: 'Sarah Aladetan, Habiba Noamany, and Coco Kneer'
---
Check out our demo [here](https://cms633cfrp.herokuapp.com/)!

![Screenshot from 2017-09-28 23-00-06.png]({{site.baseurl}}/assets/Screenshot from 2017-09-28 23-00-06.png)

We decided to approach our idea by building a web application that would take data we received from the API and display a slider that would show average ticket sales for that year and various other facts, such as the most shown play of the year. 

One of the main implementation decisions we had to make was how we display time across the 113 years. When we originally thought of our idea, we thought we would show data for every day on our timeline. Once we actually started implementing our idea, we realized that it would be unefficient to scroll through 133x365 days of data. We then decided to aggreate the data and show averages by the year, as that was much more feasible. 

We didn't end up having the time to implement this idea, but originally we also wanted to heat map the slider, so it would have changed color based the percentage of tickets sold that year as compared to the max # of tickets sold. We thought this would provide more information and tell a much more visual story.