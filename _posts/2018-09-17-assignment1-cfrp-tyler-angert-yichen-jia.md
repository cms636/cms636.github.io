---
layout: post
published: true
category: updates
title: 'Assignment1: CFRP - Tyler Angert, Yichen Jia'
author: 'Tyler Angert, Yichen Jia'
---
Presentation:
[CFRP Presentation](https://docs.google.com/presentation/d/11f8RestYXN7OCUwZOLnjimDwbmdwR9prE5ShLQmIvzY/edit?usp=sharing)

Prototype Description:

**Your approach to go from facsimile to data**

We will use a combination of computer vision based techniques and manual labelling. We can use OCR (optical character recognition) to get the raw data from the page into digital format. We are unsure of how to handle the edge cases and inconsistencies in labeling, and will likely need to manually enter in data from uncertain cases (however, the uncertain cases can be automatically grouped together).

**The process by which you will store and present data**

During the data storing and presenting process, we believe the major problems we need to address include how to cluster different types of data, how to deal with different in seating category names among different theaters, how to organizing qualitative to quantitative data,  and how to model a database to sort, organize, as well as filter. 

Because the data is highly unstructured, we will use a NoSQL database. This will allow us to easily organize the various and (perhaps unpredictable) formats of data we extract. We can also easily add new categories and data types to store on the fly. From a prototyping perspective, this also allows us to use something like Google Firebase, which is both NoSQL/document oriented and has real time functionality built in-- meaning that anybody who connects to the database gets automatic updates.

**What tools you would be building**

Our tool will represent the data from facsimile in a three-dimensional Augmented Reality environment, where the user can walk around and interact with the different theaters and their metadata. We will project the interior setting and seats layout of each of the theaters inside an empty room, with ticket data floating on top of the corresponding seats type. Students will be able to walk inside and around the interactive model, and perhaps even control the the time period by walking/moving through space.

**Who is the audience**

Audience for our project will primarily be students in history classes learning about the history of the humanities-- in this case, the history of theater in France.

**What kind of research questions does it answer?**

How can you explore time in a historical context?
How to represent data in three-dimensional space?
What impact do collaboration and community have on understanding history? 
How can immersive AR experiences increase engagement and understanding of complex material?
What impact would it have if it is used in related courses in K-12 education? 
