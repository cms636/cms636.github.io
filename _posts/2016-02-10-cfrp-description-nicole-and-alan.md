---
layout: post
published: true
author: Nicole Seo and Alan Casallas
category: updates
tags: 
  - "null"
title: "CFRP Description - Nicole Seo and Alan Casallas"
---

##Our approach to go from facsimile to data##

We plan to use human data entry to extract the data from the theatre records and store it electronically. Because the information is presented in a mostly handwritten, highly irregular form, we ruled out the possibility of using machine vision to extract the data. However, the sheer quantity of the register pages made us wary of taking a purely human-driven approach (i.e. hand-coding the data). Our strategy to make the process easier for human encoders is to group together records with similar formats and to create an electronic form with an intuitive user interface to facilitate the data entry process (see Slide #1).
 
##The process by which we will store and present the data##
We will store the data using a SQL server such as MySQL, which scales well with large amounts of data. We will store play information using database fields such as ‘Play ID’, ‘Play Name’, ‘Revenue’, ‘Expenses’, and ‘Total Attendance’. Other data, such as seats sold by section area, will contain fields such as ‘Play ID’, ‘Seat Type’, ‘Number of Seats Sold’, and ‘Revenue’.
In presenting our data, we wanted to process it in a meaningful way rather than just presenting it in a table or graph. Thus, we will create a website reminiscent of modern movie sites such as IMDB or Rotten Tomatoes that will allow the user to explore the plays as if they were modern-day productions.

##The tools we will be building##
Our website will consist of pages dedicated to each play found in the records. Each page will display information regarding the play’s ticket sales, seat distribution, revenue, and profit. By cross-referencing other sources of data, we may even present critic reviews or a story synopsis. To facilitate navigation of the site, we will include a search bar where the user can find plays by searching for their title, venue, and more. Our website homepage will show lists of ‘Top Plays’ ranked by attendance, profit, and other criteria.
We also plan on including a graphical tool with our website that will allow the user to generate custom bar graphs by selecting an independent variable, such as ‘Time’, and a dependent variable, such as ‘Total Attendance’. The generated graph would then allow the user to obtain a visual impression of the information that our data has to offer.
The front-end portions of our project would be created with the Bootstrap framework complemented by HTML. Our back-end would use a server framework such as Node.js.
 
##The audience of our project##
Our target audience will consist of scholars interested in studying the culture of French theatre during the 16th and 17th Centuries. This may include french historians, cultural scholars, and drama scholars. However, the graphically appealing nature of our website will also make it possible for non-scholars to peruse it.
 
##Potential Research Questions our Project Addresses##
Our data can be used to examine how French theatre during this era interacted with the contextual environment of the time. For example, one could study how historical events of 16th Century France, which included various wars with Great Britain and expansive colonization efforts, affected the themes and popularity of theatrical plays. Another area of study could be how theatres in France decided to allocate their expenses and how these priorities changed with time. One could also study how actor pay changed with time, or how changes in actor pay correlated to changes in ticket revenue.
