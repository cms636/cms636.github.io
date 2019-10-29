---
layout: post
published: true
category: updates
title: Updates on Wikipedia Dramatizer
author: Shiyi Peng
---
**Some updates after exploring the functions provided by Wikipedia API

How to get content by revision:

-> Get data with content for the last revision of titles API and Main Page.
action=query, prop=revisions
[https://i.imgur.com/3kUD5AM.png](https://i.imgur.com/3kUD5AM.png)

results:
[https://i.imgur.com/3zcD1Cr.png](https://i.imgur.com/3zcD1Cr.png)

other examples:
[https://www.mediawiki.org/w/api.php?action=help&modules=query%2Brevisions](https://www.mediawiki.org/w/api.php?action=help&modules=query%2Brevisions)


-> Compare two revisions from the same page
action=compare, prop=diff,diffsize
[https://www.mediawiki.org/wiki/API:Compare](https://www.mediawiki.org/wiki/API:Compare)

results:
[https://i.imgur.com/nS7XhwY.png](https://i.imgur.com/nS7XhwY.png)
