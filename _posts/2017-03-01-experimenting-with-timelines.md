---
layout: post
published: false
category: updates
title: Experimenting with Timelines
author: Peter Downs
tags: ''
---
For this project, I wanted to try out the the Knight Lab's [TimelineJS](https://timeline.knightlab.com/) tool for building interactive timelines. I'm normally more attracted to programming-heavy tools, but the point of htis class is partly to explore building tools for non-programmers: perfect.

Well, until I realized that the format the data came in didn't match the format that TimelineJS requires. Immediately I dropped into [IPython](http://ipython.org/). Using [Pandas](http://pandas.pydata.org/), I read in the original data (in a .xlsx file that I cannot otherwise open locally because my linux computer does not run Excel,) and wrote a short script to convert it into the appropriate format. The tricky part was really the date formats, everything else was a 1-1 mapping. For instance, I had to change a "Title" column to a "Headline" column -- simple.

Then, I output the data into a properly formatted `.csv` file and uploaded it to the Google Sheets spreadsheet that TimelineJS uses.

And that's it. Done! Very few other options are given. Prose won't allow me to embed an iframe, so you can [view the final result here](http://peterdowns.com/projects/timeline-example.html).

The biggest shortcoming I encountered is the lack of control over the display. If you look at the result, the events are crammed together and nearly unreadable. No events are given more visual weight than any other, so it's hard as an observer to understand what's worth reading and what isn't.