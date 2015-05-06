---
layout: post
published: true
title: Design Document Draft
category: updates
author: "Yanni Coroneos, Corey Walsh"
---

### Wubify.me

Yanni Coroneos
Massachusetts Institute of Technology, Electrical Engineering and Computer Science
Programmer
 
Corey Walsh
Massachusetts Institute of Technology, Electrical Engineering and Computer Science
Programmer



## Abstract
In this paper we will describe a novel medium for collaborative audio synthesis. By combining the achievements of previous products and taking into account the needs of the user, we have created wubify.me. We will show how users at every level of expertise can meaningfully benefit from the featureset and we especially believe that our shareable user-contributed block library can elevate the experience of audio synthesis to a social activity.

## Concept
We envision a collaborative sound generation platform, accessible through the web so that both amateurs and professionals can create sound and have fun together. There are current technologies, such as SuperCollider, that can be used to collaboratively generate sound but they are mostly a niche product that is exclusive to audio professionals who are also expert programmers. 

These technologies are powerful, and lend themselves well to our goal of sound generation, but are difficult for everyday users to access. Therefore, we decided to build a visual representation of the interface to bridge the gap in experience levels. We’re also able to leverage the nature of this visual interface to enable both real-time collaboration and a shared repository of reusable prior work.

Like some other programs, the users have a set of transfer functions that they can manipulate and compose. Filters, function generators, and even interactive elements are in the repository. A key advantage of wubify.me though is that this is all done in the browser, including the final composition step that actually plays the sounds.

## Background Research
The need for wubify.me was realized when a hobbyist electronic music composer expressed interest in a visual composition system. He complained about the current status of SuperCollider and its lack of portability. The whole system is complicated and clunky which makes it difficult for artists to distribute their work. Additionally, the complications prevent new users from entering the scene. Despite these shortcomings though, there are several things SuperCollider does extremely well.

SuperCollider is the current leader in the field of algorithmic music generation. By allowing users to create and manipulate audio signals directly in frequency space through the use of basic building blocks, electronic music composition became more accessible for everyone with a computer. The basic principle of SuperCollider carries through to wubify.me: signals are shaped through a tree of transfer functions. For example, a sine wave might go through a low pass filter which then is fed into a block to modulate the frequency of a square wave. This direct manipulation of the frequency domain gives the user complete control of the spectrum of the audio signal. By combining this approach with a conventional sequencer, like is present in Audacity or garageband, the audio signal can be completely specified in both frequency domain and in time domain. This is critical for electronically composed music which often relies on un-naturally occurring sounds and spectra.

## Project Development
Our application has a few goals:
1. Improve accessibility of existing tools
2. Utilize that improved access to allow collaboration
3. Allow for persistence and reuse of the collaborative works

To accomplish these goals, we designed and implemented a proof-of-concept application with the following basic requirements:
- A visual interface to a tool like SuperCollider
- Real-time collaboration over the internet
- A shared, persistent ‘block’ library

The basic premiss of the proposed application is such: commutations on sounds or sound generators can be represented as building blocks, and any set of composed blocks can be represented by a single block. Starting with the set of “unit generators” (“ugens”) provided by Flocking.js, users can compose blocks to create more complex sounds and processing pipelines.

This premiss lends itself well to accomplishing all three of our requirements. A visual interface must simply allow for basic graph manipulation. Real-time collaboration is done by synchronizing the states of the visual graph representation across the users’ browsers. Finally, a block library must allow users to upload the data representation of their creations to a centralized location and then serve that information to other users alongside the standard ugens.

The implementation of this project decomposes into a few parts:
- Flocking.js Representation
- Graph Representation
- User Interface - Shared block library, real time collaboration
- Web Serving
- Persistence

The primary ‘brains’ of the technology is the algorithm that converts the graph representation into the valid JSON object that Flocking.js requires. This algorithm traverses the graph, at each node it generates a corresponding Ugen descriptor, populated with default values and user specified options. Finally, it sews the fragments into a cloth that represents the network of commutations in the frequency domain.

## Enabling Technologies
Our proof-of-concept application would not be possible without the help of a long list of enabling technologies. Most notably:

**Flocking.js** - Flocking is a SuperCollider inspired JavaScript library that provides a similar interface and operation. It has the benefit of being executable in the browser - greatly simplifying the process of delivering audio output to our users

**JointJS/Rappid** - “A complete diagramming toolkit.” [1] JointJS is a JavaScript library that provides support for visualization and interaction with graphs. Rappid provides a set of higher level features that greatly sped up the development process of our proof-of-concept. While JointJS has a free and open source MPL 2.0 license, Rappid is a commercial product that was provided free of charge for our academic use.

**Node.js** - A leading, open source web-server platform written on top of Chrome’s high performance V8 JavaScript runtime. Node provides a platform for both our file serving needs and our application’s runtime requirements.

## Journey Map
Wubify.me has a straightforward UI. The user simply logs in and is presented with an empty graph and a myriad of ugens on a left side pane. As mentioned previously, ugens are like function generators; Triangle waves, sawtooth waves, and square waves are among the basic ugens currently available. The user drags a few ugen blocks into the empty space and notices that they have input and output ports. By dragging arrows from outputs to inputs, the user can cascade the ugens. Mathematically, this is equivalent to multiplying transfer functions. Each ugen can have different inputs but the most common ones are add, mul, freq, and phase. Connecting an output to each of these ports either adds the output to the base frequency, multiplies the output with the base frequency, changes the base frequency, or changes the phase angle of the target ugen block. From there the user composes ugens and then hears the result by clicking the play button. If desired, the current cascade of blocks can be saved into a new super-block in the user block library by clicking the save button.

## Future Direction
Our proof of concept application provides the basics, but we believe that this project could be taken much further. A built in sequencer would allow for more natural coordination of multiple generators. Currently, a similar effect can be achieved with multiple delay blocks and triggers, but the process could be greatly streamlined for the common use-case.

While our implementation is built on Flocking.js, only relatively minor changes would be required to make it work with SuperCollider. The UI would be virtually unchanged (aside from the available ugens); only a new graph parser would be required to generate valid SuperCollider code. The larger implementation challenge, however, would be integrating SuperCollider’s synthesis servers with the in-browser web application for near real-time sound playback.

## Works Cited
http://jointjs.com/about-rappid

http://flockingjs.org/
