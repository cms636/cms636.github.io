---
layout: post
published: false
author: ""
category: updates
tags: null
title: CFRP Visualization Project
---

Live demo: http://zygi.gitlab.io/cfrp-viz/

###Project Title
What was in vogue at the Comedie-Francaise?

###Project Team
Zygimantas Straznickas, Nicole Seo, Karrie Peterson

###Research Question: How can we enable non-experts to expore general interest trends within this data – e.g., popularity of plays, of authors, of actors? 
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

Part Two:   Design considerations for the user interface

Accolade Generator - The uncomplicated accolade generator allows users to explore the best and the worst by year.   Obstacles for doing this easily involve linking to additional data for identifying actors by gender (female/male), and singling out the leading roles for each play, so that minor characters are not tied with actors playing major roles.  Additionally, there needs to be some documentation that explains to users that the top grossing plays will be affected by play-going in many of the years, where for certain performances there were restrictions on who could attend. 
Trendline Generator - Data visualizations for longitudinal trends could be bar charts where we’re just showing absolute frequencies (number of times a play was performed, for exmple), or to show relative popularity could be unordered bubble charts or stream graphs.  


Part Three:  Use of the API to capture data

For best play and nominees:  The “top grossing play” needs to be defined and documented.  Since there were two plays on each night, attached to one gross sales amount, and we cannot determine if one was the “opening act” for a more renowned play, we chose to divide the take in half and give each play for the night 50% of the take.  Since plays were often repeated in the same year, our assumption was that a more popular play would be repeated more often, and thereby get a higher gross.  The Turkey (least grossing) would just be the same process bt lowest number.

Best in class:  Similar process, first identifying the highest grossing, and then retrieving its genre.  There would be one winner for tragedies, and one winner for comedies, in any given year. 


Top box office attraction and hardest working actor in show biz.    -->Credit to Andy Stuhl, who explained a multi-step process, as follows:

There's an API endpoint for 'participations' (http://api.cfregisters.org/participations) that serves as a link between actors (the 'people' endpoint) and register entries. The data you get from a 'participations' query will include a 'person_id' and a 'register_play_id' — these values will match up with an 'id' value in the 'people' endpoint and in the 'register_plays' endpoint, respectively. The 'register_plays' endpoint will in turn give you a 'play_id' and a 'register_id' which you can cross-reference with those endpoints, etc.

So if, for example, I want to see what plays the first actor in the data appeared in:
1) Query "http://api.cfregisters.org/people". First result is "Abeille", whose id is 316
2) Query "http://api.cfregisters.org/participations?person_id=eq.316" (note the url parameter to specify our person_id). I get two results, with register_play_id's of 45228 and 45229.
3) To get info on that first performance she appeared in, query "http://api.cfregisters.org/register_plays?id=eq.45228". I get one result, with a play_id of 18.
4) Query "http://api.cfregisters.org/plays?id=eq.18". I see that the play was "Démocrite amoureux". I can repeat steps 3 and 4 with the other register_play_id I got in step 2.

If I want $$ information instead of just the play info, I can use the register_id (29382) I got from step 3 to keep searching:
5) Query "http://api.cfregisters.org/registers?id=eq.29382". I get one result, with lots of data from the night of that specific performance, including two "total_receipts_recorded" fields that tell me the earnings.

	Favorite of the cheapskates - Play with the most parterre seats, using the endpoint “name=eq.Places de Parterres”.

Part Four: Structure of data and technologies for query and display

 