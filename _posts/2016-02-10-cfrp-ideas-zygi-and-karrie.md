---
layout: post
published: true
author: "Zygimantas Straznickas, Karrie Peterson"
category: updates
tags: 
  - "null"
title: "CFRP Ideas - Zygi and Karrie"
---



_Link to the presentation [here](https://docs.google.com/presentation/d/1wXAaZxRBsnJwrJUA6EllR2zYS2oXMSR_UwVdZAmpvkI/edit?usp=sharing)_

#### Data digitization
While the facsimiles in CFRP all list the prices and numbers of tickets sold, there isn’t a single uniform representation of this data. Because the records span more than a hundred years, there are a lot of differences in how the documents are structured and what information is included. In addition, most of the text is handwritten, which makes it impossible to fully automate the transcription process. However, optical character recognition (OCR) can still be used to speed it up by extracting all printed text from the documents. While most of the text would still have to be transcribed manually by a human, they could reference the auto-transcribed printed text and just copy and paste the words instead of having to type them.

The structure of CFRP data can be naturally represented by a relational database scheme. Each block of entries in the CFRP records represents a _PlayPair_. Because a single ticket was sometimes sold for two plays that would happed at the same evening, a _PlayPair_ would contain a title of the first play, a title of the second play, a date, and a list of _Tickets_. Each _Ticket_ object represents a group of same-type tickets sold for the same PlayPair and would contain a number of tickets in this group, their cost, and the name of their seat type. Because of inconsistent ticket type descriptions used throughout the records, it is not enough to just enter them as text since then it would be very difficult to compare them - is a _Parterre_ seat better than _Place de Parquet_? In order to make comparisons easier, it would be useful to divide all the different ticket types into a few categories and then, for each _Ticket_ group, store both the text transcription of its type and the discrete category it belongs to. This could be done by knowledgeable transcribers, although a better solution would probably be to categorize the tickets in a post-processing step.

#### Data access
The main advantage of storing the data in a relational database format is that this allows the researchers to easily query the database and get answers to many complicated questions, e.g. how many tickets have been sold to a particular play or how the total sum of ticket prices depends on the month. Because the database would probably be quite small, there would be many ways to distribute it, from simply sharing the file and letting computer-savvy researchers process it themselves, to connecting the database to a web-based graphical user interface that would make issuing interesting data queries accessible to the public. In addition to simply providing access to data, a simple web view could be designed to show each _PlayPair_ and its ticket records for people who just want to browse.

#### Data use
By itself, the CFRP data would probably only be useful to other researchers, as a data source to use in other projects. While the records could be used to explore some economics questions - how did the price of tickets or  the difference between quantities and prices of different seat types change - it lacks a lot of context for many interesting insights. The primary use of this project would be combining it with other datasets. Specifically, having more data about the plays, their playwrights, lengths and genres would let us answer questions about which genres were popular or if there were any extraordinarily popular playwrights and how much their popularity helped sell their plays. Similarly, combining the CFRP records with data about the actors in each performance could be used in research about the “superstar” status throughout history by supporting written sources with statistical data. All in all, this project would digitize and make accessible a lot of interesting data that, when combined with other sources, could then be used for exciting research.
