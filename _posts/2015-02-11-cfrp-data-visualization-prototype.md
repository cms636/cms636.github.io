---
layout: post
published: true
title: CFRP Data Visualization Prototype
category: updates
author: "Judy Chang, Ben Reynolds, GiHun Choi"
---

### From Fascimile to Data
We plan to use OCR (optical character recognition) to automate as much of the data extraction as possible. We would pair this with a crowdsourced approach such as the use of captchas to correct errors in the OCR and extract any of the handwritten text the OCR is unable to understand. 

The data we plan to collect includes: date, ticket prices, number of tickets sold, types of tickets offered, total revenue, play title, and actor names.

We also plan to manually research additional data such as the genres of each play, and the dates of major historical events that may have impacted the theater.

### Storing and Presenting the Data
We would store this data in a database such as MongoDB. Each register page would be stored as a separate entry with all of its associated data.

We would present the data in a number of ways. An interactive line plot will allow users to select certain data types and see their values plotted with respect to time: for example, users could view the total revenue over time, or the ticket prices over time.

We would also have a method for users to sort data in a ranked manner with respect to any of the data categories; for example, users can see which plays sold the most or fewest tickets.

We would also have a map of the theater that displays each section shaded in darker or lighter depending on the number of tickets sold in that section on a given timeframe. Users can select a timeframe (as narrow as a single night, or as broad as all-time), and see the relative number of seats sold in each section. Users can also filter this down by the type of play, for example comedies vs tragedies.

### Tools to Build

We can build analytical tools for our audience. For theater owners, we can have multiple cross comparisons of theater profit versus showing patterns, so they can quickly see which shows are popular at what times, and etc. This can be a collection of multiple charts where the users can choose which fields to observe. 

For researchers, a drag-and-drop graphic tool can also be built. There can be an efficient query tool for them to flip through the data, and also an easy selection tool for them to choose which columns of the data to compare and observe for patterns.

### Audience

Our exact audiences can be two types: researchers and theater owners. The researchers who are studying cultures in that time period will be greatly benefited. Plots displayed will give a clear insight on the various details the researcher may be interested about the theater and its financial status. Our approach will also be beneficial to the theater owners in that they will be able to see how certain trend developed in a specific time period. Seeing how the historical events induced the growth of a trend will be a great data for the theater owner, who can use that information and apply that on his/her theater in order to optimize the profits.

### Questions To Answer

Some questions our prototype can answer include:

- How did the historical events influenced the development of a genre in a time period?
- When did the theater make the most revenue from the ticket sales?
- Why did the theater sell the least amount of tickets at that time?
- How did the theater’s ticket prices change over time?
- Did the theater experience any sudden economic hardship?
- Did the ticket sales rise when the show featured a famous actor/actress?
- Which genre was loved by the French at all time periods?
- How did the change in theater’s design contribute to the ticket sales?