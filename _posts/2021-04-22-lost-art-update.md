---
layout: post
published: true
category: updates
title: Lost Art - Update
author: 'Mulan, Shayna, Justin'
---
**Results from Audience Research**   

Our group talked to our museum audiences Kristen, Chris, and Olga, and the general idea of exposing artworks that are less seen received positive feedback. They are very interested in the visualization of data from both instagram and museum data. It is an opportunity to be able to learn something from vast social media users, whom the museum may not be able to reach and connect before. Input from wider groups and younger audiences will allow the museum to receive more diverse feedback and comments from visitors’ behaviors and experiences. It allows them to see for example which part of the museum collection is less represented online and how the public reacts to collections and to the museum in general.
From Chris’s talk, we knew at a fairly early phase that we are not going to create a new app. We hope to use existing apps and social media, which allows both the museum and visitor to get straight into the experience without extra steps at the beginning. The museum is keen to learn more about visitors at a stage of museum transition from collection-oriented to more visitor-oriented. Chris mentioned limited use of visitor track, but there’s not much technology involved and not much learned about the visitors in the museum space. It is yet unclear how people utilize museums. Do they want to be guided (especially when they are in a big museum like MFA or have too little time to explore) or be more self-directed? Do they prefer to use smartphones or museum devices? What do they want to learn from their museum experience? What are their needs and wants and what interests them? And also why certain works are not as popular, is it because of how the museum presents them? There are tons of questions from the museum side directing toward visitors, and our project would be an interesting approach to address some of these questions.
MFA is indeed using social media platforms to create relatable contents and be socially responsible. They mainly focus on Instagram, YouTube, and LinkedIn, but at the same time they are always looking for experimental and innovative approaches.
Kristen and Chris seem to be very interested in the game idea that we have, which is basically a call to exploration in the physical museum space, allowing visitors to move around and engage with less viewed artworks. The game has an exploratory nature, which is important because people tend to stick to what they already know.
The not on viewed objects were also brought up several times in the conversation. MFA has a huge amount of art collections that are not on view, especially works that can only be out for several months every decade. The presence of these works is something that we hope to explore in the future, hopefully with the help of data from the museum.


**Technology Updates**   

Our technical development is spread between 3 main areas: data scraping/ collection, analysis, and front-end development. We currently have a dataset of all on-view works at the MFA which is semi-cleaned, and roughly 20,000 Instagram photos tagged with the MFA's account. Using the creator name for each work, we've compiled a list of MFA artists/ works that were mentioned in Instagram post caption and the number of photos associated with them. Two challenges that have emerged thus far are 1) getting a complete set of 2019 Instagram data (it's taking longer than expected due to bot detection/ blocking) 2) only items in the permanent collection are accessible on the MFA database (so even though there are a lot of Basquiat shares, we currently can't detect these without manually adding this to our MFA dataset)

We've been analyzing this data to create metrics on which works visitor's share on Instagram at the museum. One interesting finding is that isn't a strong correlation between the number of works by an artist in the museum and the number of Instagram shares. For instance, John Singer Copley has around 30 works in the museum, however Jackson Pollock's has only 2 and has more shares. Another finding is that the America's exhibit, which contains the most number of works, also has the largest amount of Instagram photos. It might be interesting to explore this further to see if Instagram shares are siloed to certain areas spatially in the museum— If so, this could open an opportunity to guide visitors toward other less-visited collections.

Using this analysis, we've compiled a list of metrics that might be useful for curators or visitors. These will be incorporated into the data exploration website. We're currently in the design process and think we will have a static version (image) of this for the final prototype. We've also been further designing and researching the data-driven curation website where visitors can view/ follow meta-tours created using the Instagram data. Olga referred us to a virtual tour app currently used by the museum (and developed by Cuseum) that shares a lot of the same functionality we've been designing. This has been helpful as we iterating on our prototype for this site.




**Short Writeup of Project Progress**   

Previously we had spoken to Kristen Gresh and Chris Atkins from the MFA to gather some of their insights on our project and the MFA’s interest.

Shayna visited the MFA galleries on 4/10 and took pictures and notes from their experience. Images are in this folder: [https://drive.google.com/drive/u/4/folders/1-0EXBbktHu5_hxebYU5b1Dm5oHmINS-h](https://drive.google.com/drive/u/4/folders/1-0EXBbktHu5_hxebYU5b1Dm5oHmINS-h )
Notably, the museum has adapted to pandemic times with directed floor flow markings that often go backwards to the implied viewing order of galleries, signalling that there is ability to suggest unconventional art viewings, such as our proposed “playlists” of meta-collections of art.
While visiting, Shayna noticed not many visitors with their phones out, with little to no use of the underpromoted MFA app. Olga remarked in our conversation that they desired to have the galleries be a comfortable space that invites such picture taking and interaction and that some of the piece descriptions were available on the MFA app in pandemic times to prevent crowding.

On Friday, we spoke to Olga Khvan, part of the social media team at the MFA, to ask about visitor engagement on social media. We found that many curators wanted to have digital aspects in their exhibitions and social media campaigns, but having seamless engagement and interaction was harder to come by. She was also interested in the photographed art frequency aggregation stats collected by Justin and recognized some of the shortcomings of social media interactions like confusion about what’s on display when it is posted on the MFA instagram and priorities as such. We may be referred to one of her colleagues to talk further.

All throughout, we have continued updating and iterating on our Miro board. We have started designing mockups of a webapp with a clean design similar to the MFA website and app aesthetics and a possible Instagram bot. We assigned tasks to group members to design and develop the webapp to bring this to prototype in the next week. Justin has continued scraping data from the MFA’s hashtag, account tag, and location tag on Instagram, albeit sometimes with blocked accounts from accessing information too quickly on the platform.
