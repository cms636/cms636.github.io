---
layout: post
published: true
category: updates
title: Museum Project Idea
author: Audrey Cui
---
(Un)finishing Touches

In the traditional art museum, interaction between the museumgoer and the exhibit is often limited by “do not touch” signs, glass walls, and rope barriers. As a result, exhibits become “untouchable,” physically and possibly also socially. Through an augmented reality app that allows users to virtually graffiti exhibits (and possibly collaborate on graffiti with other museumgoers), we can disrupt the idea of untouchable exhibits. Museumgoers are not only encouraged to (digitally) touch exhibits, but add their individual creativity to them and as some people might consider, ‘vandalize’ them. I’d expect that some users would intentionally artistically augment exhibits, whereas others would intentionally mess around with them, such as drawing comical mustaches on figures’ faces. This begs the question, when is graffiti and street art considered “art,” and when is it considered “vandalism”? 

The audience would be for all museumgoers — it would be interesting to see whether/how different demographics would contribute graffiti differently. The intended museum collaborator would be an art museum such as the Boston MFA. 

To be honest, I’ve never developed a mobile app before (just a web app through the web.lab course), so I am not 100% sure about the technological approach. User authentication and a database will be needed to store individual users’ augmentations. ReactJS and HTML/CSS can be used to build a dynamic frontend. In a web app, HTML canvas can be used as a drawing interface, and chances are there’s something similar for mobile apps. There are probably libraries out there for integrating AR in a mobile app. Someone in Borderline (AR murals club) is developing an AR app, so I could possibly ask them for pointers. Skill sets include app development and background/field research on critical examination of graffiti in the context of art and society.

Updates: After Thursday's class, I realized that another potential direction that this can go in is leveraging style transfer models to transfer the style of one museum artwork onto the content of another via an AR overlay. Because style transfer is already pretty established, I'm willing to bet that there's an API/library out there that does it for you. If not, there are's definitely open source models that can be deployed onto a cloud platform that can be called in a web app. There's already a lot of existing web/mobile apps that do style transfer for custom images, but I haven't seen style transfer being used as a participatory element in a museum setting. My ideas are similar to that of Georgia's in that we both proposed participatory AR apps that involve user contribution and possibly collaboration between different users. 
