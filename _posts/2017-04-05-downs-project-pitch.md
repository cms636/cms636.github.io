---
layout: post
published: true
category: updates
title: 'Whistle: A Modular Textual Analysis Tool'
author: Peter Downs
tags: ''
---
### Problem Statement
Various different tools exist to analyze a text (document) as a single work or a group of texts (corpus) and the relations between them. Some well known examples are [Voyant](http://voyant-tools.org) and [Tesserae](http://tesserae.caset.buffalo.edu/). These tools use computational techniques to augment humanistic research of texts. But they're limited in that they're not designed to work together; the analysis that Tesserae performs is not available to any tools in the Voyant suite, for example. I propose the construction of **Whistle**, a modular software tool that allows for many types of computational analyses, and then makes those results available to many different types of visual display. This facilitates the separation of analysis components and visualization components, which will lead to more composable and re-usable tools in the field of textual analysis, and ultimately provide humanists with better digital research aids.

### Approach
The end result will be a web-based application for text analysis. It will allow users to manage texts and group them into corpuses, and offer a variety of tools that can operate on those texts and/or corpuses. We will focus on the creation of a single analysis tool (using [fastText](https://github.com/facebookresearch/fastText) to output word vectors) and visual display thereof (finding similar phrases across documents, similar to Tesserae). But the system will be engineered in such a way that other tools can be added (both analytical and visual), and given sufficient time/resources, we would like to add those, too.

### Audience
There are two audiences. One is toolmakers and software engineers who are interested in creating novel textual analysis tools. The second is humanistic researchers who would like to use these tools without having to understand the details of their implementation.

### Skills Needed
- **Software engineering**: this project will most likely be written in Javascript from front-to-back, for development ease and speed, although analysis tools may be written in or use tools written in other languages.
- **UI/UX design**: many digital humanities tools suffer from difficult-to-use interfaces. Ideally our end result will buck the trend.