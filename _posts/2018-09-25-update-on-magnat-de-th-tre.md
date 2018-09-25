---
layout: post
published: true
category: updates
title: Update on Magnat de Théâtre
author: 'Caspar, Priya, Zidane'
---
![Screen Shot 2018-09-25 at 11.19.06 .png]({{site.baseurl}}/assets/Screen Shot 2018-09-25 at 11.19.06 .png)


After a huge struggle to actually get access to the data (Java didn't like to import the JSON tools, so we eventually moved over to Python, which didn't want to install the necessary library to fetch data directly from the API, but would at least read pre-downloaded JSONs), we managed to crunch a few numbers.

However, we quickly realized, after having read the Wikipedia page for the French Livre, that any rudimentary economic analysis would probably be a waste of time, because of the highly fluctuating value of the livre, and difficulty knowing exactly which unit of currency the prices were recorded in. The different seating categories were also difficult to access and analyze, so what we ended up with was looking at "how popular were each of these plays, probably".

To get a popularity score (not corrected for inflation, otherwise fluctuating currency value, expenses or really anything), we added up the income for each play, and divided that by the number of times that play was performed. This would most probably give an advantage to plays performed later in the time period, but the world isn't ideal. 

The advantage to this is that by using the avarage income of each play, compared with eg the total score (which was available in another JSON), is that this method wouldn't benefit mediocrely popular plays that were performed all the time, or give the impression that plays that were only performed a few times were incredibly unpopular.

Had we gotten the Java JSON import to work, this could have been implemented into our game to give the player an accurate choice of plays, and a more realistic price level.

Further, using the same dataset, we could see how the same plays would perform better or worse over time, thus giving the player even more accurate information.