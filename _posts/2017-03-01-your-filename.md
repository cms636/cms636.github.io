---
layout: post
published: true
category: updates
title: Chamberlin Mini-Project
author: Thatcher Chamberlin
---
(not sure if this is the right place to put this, but here it is)

##Mini-Project: Representing Time

![breve.png]({{site.baseurl}}/assets/breve.png)

I chose to examine the Breve web app. I found it to be not at all suited to the task of displaying the information in the US-Iran Missed Opportunities information. Each event is presented in the exact same way - as a small slice of time which each parameter (dates, title, description, location, etc) printed out next to a slice which it is clicked. 

One huge improvement here would be for the app to make each event start on its start date and end on its end date. I'm not sure why that's not a feature. The app offers very few options on how to display the data. The only way information is shown in the timeline is as text which can be read when each event is selected. There is no visual indication that some events are longer than other, occur in difference places, or are more significant. 

One thing I would like to add would be a zoom-type feature. There are over 500 rows in the spreadsheet I used and there are also three others. If each event is given its own space on the visualization, it will be hard to interpret what's going on. Instead, I think a good approach would be to give the view the ability to zoom out from the collection of events and see broader trends. One way to do this would be to cluster events as you zoom out and label them with the most common keywords shared in a set of events. For example, zooming out over late 2003 would cause the many events in the time to merge into one box with the words "nuclear", "IAEA", and "Khatami". This would give the viewer a higher-level view of the situation by showing the themes and major players over a period. Understanding will come more quickly when the visualization shows that nuclear matters were being discussed in this period instead of just showing the forty events that occurred in that time and waiting for the viewer to synthesize the events into a more complete picture. 

Another nice addition would be a visual indication of the source. In this data set there is a finite number of sources. I would like to have a way to assign them each a color so that I could tell, for example, which sources came from within the US and which came from Iran and which came from foreign observers not involved in the events.

I think the sliding timeline with multiple stacked rows is a good base concept, but it needs to be extended to effectively present this information. The zoom feature is the most important improvement, but the ability to change the display style as a function of the event's parameters be nice as well.
