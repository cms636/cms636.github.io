---
layout: post
published: true
category: updates
title: Updates to Wikipedia Dramatizer
author: Will Freudenheim
---
Slightly new format using the Wikipedia API
1. Type in a Wikipedia page name
2. Set in two dates, it'll generate a JSON that includes comments, timestamps, and users, amount of data that was deleted or added per edit
3.Processing script builds a query to Wikipedia API from this info.
4. Script parses this JSON for /* Section */ - will tell you when someone is editing a distinct section of an article and add those items to a new list.

From this new list we can build a dashboard that gives different metrics of "controversy" that describe each section of a wikipedia page.

- look at distinct sections and which areas had the most individual edits
- look at which sections were edited by the most people
- look at sections based on how much actual content was added or erased in this time: which could be a valuable measure of controversy. Sections that have nearly a 1:1 ratio of adds:erases while also having the most total number of characters added or erased means that they were more rapidly edited

This will involve some simple data manipulation based on the lists generated to find these values. Using MediaWiki's API Sandbox tool has been incredibly useful in figuring out what's possible with their API and easily experimenting with parameters.

Here's a sample of a single element from the JSON.
![]({{site.baseurl}}/assets/Screen%20Shot%202019-10-22%20at%2011.26.24%20AM.png)

Additionally, this could allow for comparing multiple pages! We could compile the metrics for each section to have an aggregate metric for each page, and use this to compare multiple pages with the same three main metrics for controversy.