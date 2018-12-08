---
layout: post
published: true
category: updates
title: Ternion Draft
author: Ternion
tags: ''
---
##  Project description
A physical data visualization comparing the texts of Islam, Christianity, and Judaism.

## Concept Overview
(core ideas, research questions, audiences, approach,etc.)

The primary inspiration from Ternion came from a very simple question-- “how do we compare religion?” We believe that the religions we chose are more similar than they are different so we took the task of analyzing the core texts from each religion to open up a discussion about these similarities. Our approach consisted of analyzing shared context between the three religions we chose: Christianity, Islam, and Judaism.
 
Our audience is everyone who is religious or is interested enough in religion to take part in our project. We live in a world where many divisions are being placed among different religions, and we wanted to create an interactive way to show people how similar their beliefs could prove to be. By making a physical and not a completely digital approach, we abstracted the underlying technology away, so that users could focus more on the message being conveyed.

The three Abrahamic Religions—Christianity, Islam, and Judaism—all hold the monotheistic belief that there is only one God. The monotheistic root of each religion has for centuries, raised curiosity amongst religious enthusiasts, researchers, and theologists. Making the quest to understand the commonalities and distinctions between the three religions one that is central to understanding humanities. 

Misconceptions about religious differences have been the root causation of many global disagreements that have led to wars, isolation, and additional human conflicts. However, amid these misconceptions lie the reality that many of these religions have similarities far beyond what has already been explored. Typical explorations of the commonalities and contrast between religions, mainly the monotheistic religions, have resulted in the creation of Venn-diagrams, table charts, and a myriad of research papers. However, a physical representation of commonalities across the religions has yet to be accomplished. For this project we will display common concepts across the Abrahamic religions through a physical means. In doing so we hope to give individuals the ability to see religion through a different lens and look towards understanding and identifying connections that have yet to be uncovered. 



## Background Research
(other models/projects you looked at, literature review, etc.)

First, we looked at traditional ways people have visualized religious texts. Most of these include graphs that compare word frequency without consideration for context. 

## Literature review:

From a computational perspective, our techniques were inspired by previous work done in Natural Language Processing (NLP), a subfield of machine learning focused on using analyzing natural language. Specifically, recent developments in Distributional Semantics-- a research area that focuses on understanding semantic similarities in language-- have allowed us to see what “context” looks like by visualizing vector representations of words, using an algorithm called Word2Vec.

Scholars have been using other algorithms like LDA (Latent Dirichlet Allocation) to cluster overall topics found in religious texts, but to our knowledge, little work has been done using Word2Vec to visualize how context changes across the religions with shared words. We found that the Abrahamic religions were the perfect candidates to see how common themes- like faith and belief, change context between texts.

Our visualizations were inspired by “traditional” visualizations of Word2Vec that show the spatial relationships between word vectors. 

Data collection:
1.	King James version for Old Testament & New Testament 
2.	Abdullah Yusuf Ali version of the Quran (references needed)’


## Project Development

### Problem & Hypothesis:
Religion has been something historically used to both unite and divide people. Through our physical interpretation of religious commonalities, we can now provide individuals with a unique medium to discover unique connections across the three religions. 

Users will be able to see clear connections across concepts in 3 distinct religions. Users will also be able to observe clear distinctions and make their own interpretations on the ways these religions resemble/contrast one another. 



1.	Started off with wanting a large, physically interactive space with digital visualizations (kinect + projection + spatial design)

![pic1.jpg]({{site.baseurl}}/assets/pic1.jpg)

2.	Technical limitations
3.	Boiling down the main part of the visualization and problem to address
4.	Choosing a small scale interactive design
5.	Brainstorming physical visualizations that don’t necessitate an interactive digital component

![pic3.jpg]({{site.baseurl}}/assets/pic3.jpg)

![pic4.jpg]({{site.baseurl}}/assets/pic4.jpg)

![pic5.jpg]({{site.baseurl}}/assets/pic5.jpg)

## Enabling Technologies

-	Data visualization and data processing
-	Natural language processing
-	Word2Vec( +diagram /screenshot)
-	LDA ( +diagram /screenshot)
-	Choice of words (logic behind it → we need to figure it out )
-	3D modeling and design
-	Rhino 


## Journey Map
Ternion will be placed at the eye level where the user can look inside the rectangular shape to have a perspective on 3 consecutive transparent lens. 

The viewer will be able to see the geometry that the chosen word constitutes with the five close words to it on the word2vec model. 

The visual comparison that the viewer is able to constitute in his mind while looking as these shapes extracted will help identify the degree of intersection of the religion at the semantic level and therefore the conceptual connotation to what degree they differ. 
Dragging the acrylic along the slits will help highlight the different words which will be lit by LED light strips inside.

We chose a grand list of words to process and compare the geometries of. These were:

['birth', 'trust', 'remember', 'experience', 'dream', 'god', 'heaven', 'hell', 'love', 'hate', 'free', 'vision', 'believe',  'light', 'forget', 'darkness', 'peace', 'war', 'life', 'death', 'man', 'woman', 'child', 'eat']

We decided to focus on having our words focus on a time-related theme, where “believe” is the center panel and represents the present. The surrounding panels represent the past and the future. 

Past: remember, forget
Present:  belief
Future: vision, faith


## Future Directions 
Moving forward, we would like to visit some ideas we had but chose to discard because of their time complexity. These discarded approaches will give the users the power to choose words, texts, and other factors to make the experiences more immersive. We would also like to explore more religious texts and analyze more data to arrive at better conclusions.

## Work cited
Word2Vec and NLP papers
