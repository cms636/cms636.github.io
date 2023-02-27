---
layout: post
published: true
category: updates
title: AI Based Collection Map
author: Andrew Stoddard
---
**A description of the issue/problem that you are trying to address**
Museums have a vast collection, much of which is never seen by the general public. Most people don’t know anything about the collection, and often the collection is so large it is hard to comprehend the scope of it. I propose a solution that allows both curators and visitors to explore the entire collection, as plotted in 2D space. This would catalog various features of the work, and then use GPT3 to create embeddings of each work, that can then be reduced to two dimensions and seen visually. You would be able to see clusters of works, and see how all of the works in the collection relate to each other. You can also explore the collection over time, and see this map for different time periods of the exhibition. It could also show when various works were on display, if ever.
![Screenshot 2023-02-27 at 12.28.20 PM.png]({{site.baseurl}}/assets/Screenshot 2023-02-27 at 12.28.20 PM.png)

**The envisioned audience for your project**
Museum Curators - use the tool to look for “gaps” in the collection (what else should be collected), or parts of the collection that have been underused. This can be used to design new exhibitions or make new connections between various works. 

Museum Visitors - this can also be used as a visualization tool for the general public - they can zoom in and out of the collection, and see how it expands over time. This is a great first step at making the scope and scale of the collection accessible to the public.

**Potential museum collaborators (currently MFA; Harvard Art Museums, MIT-Museum, and others are possible as well)**
Harvard already has a fantastic API that has information about all of the works in their collections. This would make the project vastly easier if the museum already has an API that can be used to query into the collection.

**Technological/spatial/installation approach (if part of the project)**
Use GPT-3 to create embeddings for all of the works
Dimensions reduce this embedding to two dimensions
Plot all of the data in two dimensions, and use GPT-3 to create labels for each “section” of the map automatically
Create timeline and search features for the map

**Skill sets needed for your project**
AI Coding (using GPT3 api)
Data analysis (what features of the works do we want to focus on)
Data visualization (React, D3, js)

