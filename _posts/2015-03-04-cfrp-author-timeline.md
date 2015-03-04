---
layout: post
published: false
title: CFRP Author Timeline
category: updates
---

### Research Question: Who were the authors of the Comédie-Française?
**Harihar Subramanyam, Sherry Ren, Ariana Eisenstein**

To answer our research question we have created a website mimicking the Internet Movie Database (IMDB) except for the playwrights of the Comédie-Française. Each playwright and their work is catalogued to be searched and viewed quickly.

There will be two primary ways to search this database. First, a standard search of the playwrights present in the CF data. A second option is to locate specific authors along the timeline displayed on the main page of the website. Each author is marked at their date of birth. Searching a specific year causes the timeline to display the span of ten-years from the query. This method helps contextualize the authors’ work by graphically showing the period in which they were alive, allowing the user to view which playwrights were contemporaries as well as understand the historical influences which  may have influenced their work. We found that initially the granularity of ten year periods resulted in an uncluttered visualization, which still displayed popularity trends, but that future iterations could include the option to change this scale. Additionally, we would include the ability to search plays as well as authors as well as the ability to scroll through the timeline. The initial mockup is shown below:

![mockup 1](/assets/timeline_mockup1.png)

After clicking on a specific author, the CF API is queried and the web page displays the authors lifespan, plays written, and total number of performances, which are pulled from the API in real time.  The individual playwrights pages add more details such as the popularity of their work as well as their prolificness. It further contextualizes their work as it shown when the playwright was alive. A final iteration would show a graph detailing the number of tickets each type of ticket sold for each play, mapped against the year [Figure 2]. This graph will allow users to gauge which play was most popular and when it was playing. Outside sources of information, such as a link to the text of each play or a link to a biographical reference to each author, could be included on the individual author page as well. Another mockup is shown below:



The website can be found at: https://infinite-tor-5541.herokuapp.com/. A screenshot of the website is shown below.

![timeline screenshot](/assets/author_timeline_screnshot.png)

When an author is selected (either by searching or clicking on timeline), their page appears (shown below).

![author page](/assets/author_page.png)

Authors appear multiple times in the dataset (ex. "Voltaire", "Voltaire (François-Marie Arouet dit )"), but our project corrects for this and retreives all plays for the given author and computes the total number of performances for the given author. THe birthdate and deathdate were scraped from Wikipedia.


