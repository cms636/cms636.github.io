---
layout: post
published: true
category: updates
title: Wikipedia Dramatizer 11-12 Update
author: 'Will Freudenheim, Shiyi Peng'
---
New updates to the Wikipedia Dramatizer include much of the details mentioned as the next steps in class last week. The main updates that are visible are that the user can choose start and end dates for the range of edits that will be pulled from wikipedia, rather than automatically pulling the most recent ones.

Entering a new search will automatically clear the previous search details and build a new list, while keeping the previous graph on screen. Once the graph is slightly more legible with the titles this will be much more useful for doing quick comparisons. I was already able to do some interesting edit comparisons already, even looking at the same page but in different time ranges– just looking at the Global warming page at different years shows a spread of different areas that people were working.

I also added much more detail to the section class, such that each section contains a list of the number of editors, and each editor contains both a number value for the number of edits they made to that section, as well as a list of what their comments were along with each edit. This isn't implemented visually in the code yet, but the design is there, which you can see in the console. Our main next step is displaying this more granular information graphically when someone clicks on one of the bars on the bar chart. Here is an example of the output of the six people who edited Donald Trump's section on wealth in the past year, which includes the number of edits that each person worked on and the content of each edit.

![Screen Shot 2019-11-12 at 7.42.22 AM.png]({{site.baseurl}}/assets/Screen Shot 2019-11-12 at 7.42.22 AM.png)


One challenge that I'm not totally sure how to deal with is the case sensitivity with Wikipedia. The casing is not universal, where for proper nouns like names they expect all of the words to start with a capital letter (ie Donald Trump) but for other words generally, the first word should be capitalized, but the rest remain in lower case (ie Global warming). I don't see any way of automatically detecting how to fix casing issues when someone is entering their information, given that I won't be able to tell what kind of thing it is they're searching for. But perhaps there is some lookup I can do using the Wikipedia search with their terms, and pull from the resulting URL. Will need to do some more research here.