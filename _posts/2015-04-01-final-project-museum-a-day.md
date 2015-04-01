---
layout: post
published: true
title: "Final Project - Museum a Day"
category: updates
author: Zach Sherin
---

I'm not great at outlining these so I'm just going to follow the sections outlined in the handout:

**Problem Statement:**

Museums can be difficult to approach, occaisionally pretentious, and often expensive or difficult to get to. Also, many museums feature only works that could be considered "fine art" or otherwise well-known pieces in an accepted, established style. I want to create a museum that is easy to access, open to all types of artistic works, and most importantly, free.

**Approach:**

The Museum a Day project is a virtual museum, automatically generated or hand-curated in special circumstances, that can either be explored in a browser or through the use of a Google Cardboard headset and a phone. I will cover the automated case, as a hand-curated museum is fairly easy to imagine. 

First, we gather art through a web-scraper, not only from established gallery websites that contain images and data on fine art, but also from websites such as DeviantArt, to gain a mixture of classically expected museum art, and strange, unconvential art from creators on the Internet. 

Next, using a set of predefined "museum rooms" that the team creates the system will generate a museum and populate the rooms with the selected art. This can be thought of as having a bunch of empty rooms with defined "art spots" and then mixing and matching until a museum is made and filling the rooms by sorting art according to some clustering or semantic matching algorithm. The algorithm to determine what art goes together in what rooms should be thought of as building a virtual curator. It could care about metadata attached to the art (tags, descriptions) or maybe the visuals of the art itself (clustering similarly colored, composed, etc art). That is more a question for the group to answer together, though.

Finally, the newly-created museum will be uploaded to a server, where users with the app can download it and view it in 3D on their phones, or else use a browser to access the museum. In this way, we'll have created a museum with a very different collection of art that is accessible to anyone with an Internet connection (which, of course, is not everyone).

**Audience:**

The audience for this project is mainly a younger audience, probably under 30. The reason I say this is that not only does accessing Museum a Day require finding a technologically-accessed museum interesting, the museum itself will be populated by a mixture of classical art and strange art collected on the Internet. I personally feel that appeals to a younger, more technologically-focused group of people who would be interested in seeing art but perhaps not interested in going to a museum.

**Skills Needed:**

Web Scraping: I am not a web developer, and the methodology for automatically finding and acquiring artwork from the Internet is a task that frankly leaves me very scared. I'm sure it's not impossible, it's just outside of my realm of expertise

Designing Museum Rooms: I would like the museum rooms to be hand-created, rather than automatically generated. This way I think they'll look nicer. I'm not a great designer, and someone with an eye towards architecture/user experience could perhaps have a better idea of how to build the museum rooms so that they fit together nicely.

Building the game/museum generator: This I am good at. I have built many games and particularly am proficient with the Unity3d game engine, which supports Google Cardboard and browser interaction. 

Building a server to host the Museum a Day: I don't know much about servers and websites, so someone (perhaps the web scraping specialist as well?) who enjoys putting together a website that could deliver the Museum a Day would be great. 

That's the Museum a Day. I'd love to work on it, and I hope maybe others are interested as well.