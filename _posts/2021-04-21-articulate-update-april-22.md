---
layout: post
published: true
category: updates
title: ARticulate update April 22
author: 'Audrey, Trevor, and Georgia'
---
**Introduction**
ARticulate is a mobile tool that allows museumgoers to participate in the public commentary. Visitors can choose to engage with art pieces in two ways. First, visitors can create responses. This entails annotating a piece in AR, writing a short piece of text to support the annotation, and tagging that response. For certain pieces or exhibits, we would like to enable the curator to provide a prompt or question to visitors to respond to. For other pieces, freeform response would still be available. In the second interaction mode, visitors can view others’ responses, filtering by tags if desired. Here, they can respond using emoji reactions. 

**Reserach**
Interviews with MFA staff and museum goers have told us that different visitors will choose to engage differently. Some people will prefer to read others’ responses first, and some people prefer to create responses first. Because of that, we are equally prioritizing these two paths of engagement. 

We have seen how ARticulate could provide benefit to both museum goers and the museum staff. Museum goers will be able to engage with art in a new way. Other modes of providing visitor feedback and responses exist, but with ARticulate, visitors are able to visually annotate a piece in AR. This is a new function that brings a visitor’s engagement even closer to the original piece. Being able to see others’ commentary allows visitors to see a diverse set of modern viewpoints. This is often missing in many exhibits. 

Museum staff will be able to collect more data about how visitors are responding to their pieces and exhibits. Some exhibits already implement a Post-It note interaction where visitors respond to a curator-promoted question. The Post-Its are then sorted, and some are displayed on a wall. The MFA staff thought this was a very effective part of the exhibit. Articulate allows museum staff to take this type of interaction one step further. There is no physical limit to how many responses can be displayed, so all responses are available. Further, the visual AR annotations provide a new way to react to the artwork that Post-Its don’t. 

MFA staff who focus on social media engagement have been asked by museum leadership to share visitor testimonials on their platforms. ARticulate provides a great tool for collecting these testimonials or responses. In one interview, an MFA staff member said she could imagine using visitor-generated poetry as an Instagram caption to a post highlighting one of the pieces in the museum. 

Visitors will primarily use their personal device to use ARticulate, but museum-owned devices will be available to ensure everyone has access to this tool. This is in line with what the MFA currently offers.

**UI/UX**
Based on feedback from classmates and from MFA staff, we updated our UI/UX to prompt the user to add personal info tags such as age when they first use the app, tag their response with content identifiers, and filter responses via the tags. The current Figma prototype can be accessed [here](https://www.figma.com/proto/qWZ8ITvQK8M2P9pIW4IeyA/ARticulate?node-id=9%3A2&scaling=scale-down&page-id=0%3A1). 

We recently decided that users cannot respond to initial responses via text, but rather only via emoji reacts in order to decrease the amount of moderation needed. We plan to update the wireframe accordingly, and continue discussing ways to streamline the interface. 

**Technology**
ARticulate will be distributed to smartphones and tablets. These could be either visitor owned or museum provided devices based on what any museum partner feels is best for their needs.

The foundation of the app will be built with a game engine called Unity. This is what we'll use to implement the UI, write custom behavior, and link together the different third party tools we're using. We currently have a functional prototype developed with Unity and will continue to iterate on that.

For the generic augmented reality functionality, we're using an SDK called Vuforia. We compared Vuforia to Unity's in-house tool, AR Foundation, and found that Vuforia had enough of an edge in effectiveness and documentation to justify using an external tool.

User generated content will be saved and retrieved in two parts. The visual portions of users' annotation will be saved as images while the rest of the data (text annotation, content tags, demographic tags, etc) will be bundled together and saved along with a link to the image if applicable. When viewing annotations, our current plan is to interact only with the text based data to sort and cycle through annotations. Once users have selected a set of tags or opted to view completely random annotations, we'll download the image data for each annotation only when it's being viewed. Both forms of data will probably be stored on AWS but in different systems. The text data will need to use a database while the images will likely just be stored in an S3 bucket.
