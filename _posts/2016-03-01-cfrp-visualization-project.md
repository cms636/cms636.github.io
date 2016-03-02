---
layout: post
published: false
author: ""
category: updates
tags: null
title: CFRP Visualization Project
---

Live demo: http://zygi.gitlab.io/cfrp-viz/

##What was in vogue at the Comedie-Francaise?

###Project Team
Zygimantas Straznickas, Nicole Seo, Karrie Peterson

###Research Question
How can we enable non-experts to expore general interest trends within this data – e.g., popularity of plays, of authors, of actors? 

Today’s audiences often think in terms of awards, box office profits, top-billed celebrity performers.  To provide entree to this historical data, we are attempting to enable exploration in those kinds of categories.

###Functionality of the web-based interface

We aimed at giving users the ability to discover year-by-year information using an Accolade Generator:

Best play – Highest grossing play
Nominees – Top ten highest grossing plays
Best in class – highest grossing in each genre  (comedy, tragedy)
Most popular playwright – authors of the top grossing play
Nominees for playwrights - authors of the runners up
Top box office attraction - actors/actresses whose appearances total up to top grossing numbers
Hardest working actor in show biz - actor participating in the most plays in a given year
Turkey – least grossing play
Favorite of the cheapskates – play for which the most number of the cheapest seats sold for that year
 
More complex data extractions could permit:	
Mood of the season - showing the proportion of comedies vs. tragedies for each season of a given year 
Longitudinal summaries of individual plays, actors, playwrights over a period of time, showing their frequencies.

Longitudinal playwright popularity:  Allow users to view the relative popularity of playwrights in a designated time period.  Users can choose any time period, and get a visualization that shows each playwright whose plays were performed in that time period as a circle, with the size of each circle increasing based on total gross.  If the time periods are very small, it might not be so important to correct for the change in the value of currency over time, but if the time periods were large, that correction would be needed.
Design considerations for the user interface

Accolade Generator - The uncomplicated accolade generator allows users to explore the best and the worst by year.   Obstacles for doing this easily involve linking to additional data for identifying actors by gender (female/male), and singling out the leading roles for each play, so that minor characters are not tied with actors playing major roles.  Additionally, there needs to be some documentation that explains to users that the top grossing plays will be affected by play-going in many of the years, where for certain performances there were restrictions on who could attend. 
Trendline Generator - Data visualizations for longitudinal trends could be bar charts where we’re just showing absolute frequencies (number of times a play was performed, for exmple), or to show relative popularity could be unordered bubble charts or stream graphs.  

###Use of the API to capture data
For best play and nominees:  The “top grossing play” needs to be defined and documented.  Since there were two plays on each night, attached to one gross sales amount, and we cannot determine if one was the “opening act” for a more renowned play, we chose to divide the take in half and give each play for the night 50% of the take.  Since plays were often repeated in the same year, our assumption was that a more popular play would be repeated more often, and thereby get a higher gross.  The Turkey (least grossing) would just be the same process but lowest number.

Best in class:  Similar process, first identifying the highest grossing, and then retrieving its genre.  There would be one winner for tragedies, and one winner for comedies, in any given year. 

Top box office attraction and hardest working actor in show biz: it would be difficult to implement this using just the API provided - even though there are API endpoints for actors and their performances, in order to correlate them with performance profits it would require getting information about all the different combinations of performance and actor data. This can only be achieved by first using the API to download all the actor data in the project and all the performance data for each year (assuming that's not against the terms of use) and then processing the whole dataset. 

###Structure of data and technologies for query and display
For display, we would use a simple jQuery based script to display the top 10 lists and control the website. Graphs would be drawn using the d3 library. The data retrieval question is more complicated. In our demo, we only implemented the worst/best plays functionality, the data for which could be retrieved using a single API call to the CFRP server. For this, we just used an AJAX call from the user's browser - the website does not need any functionality from a separate backend server as everything is done clientside, by the browser. When implementing other views, specifically the "hardest working actor" category, a different approach would be needed. As Described above, this data cannot be acquired by a single API call. The project would need a backend server that would collect all the data needed by doing many API calls to CFRP, processing them, deriving the statistical data and then serving it to the website visitors.

 