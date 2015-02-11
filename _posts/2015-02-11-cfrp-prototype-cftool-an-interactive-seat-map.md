---
layout: post
published: true
title: "CFRP Prototype – CFTool: An Interactive Seat-Map"
category: updates
author: Deniz Aksel
---


##Main Idea:
Data visualization is a very powerful tool that can allow an observer to comprehend and interpret mass amounts of information within a short observation time. This is why my project aims to summarize the data stored in facimiles from the Comédie-Française Theater in a visual manner.  I believe that an interactive map of the theater would not only help display knowledge relating to the attendance and pricing history of the theater in a intuitive fashion, but added features can make the data very accessible and flexible to various interpretations.

## Data Extraction from Facimiles:
As seen in the four sample facimiles, the structure of data storage has gone through many variations over the 113-year time span. As a result, simply processing the data via OCR will likely not be sufficient for data extraction. A good approach to digitizing the data might involve:

**1)	A crude categorization of the documentation into different data storage formats:** Using feature recognition, the scanned image files for the facimiles can be separated into clusters that have an overall similar outline. 
**2)	Labeling regions within the image with the relevant data:** With knowledge on the various different formats, we can now label each format with ROIs defining the nature of the information stored in that portion of the page.
**3)	OCR:** the text can be digitized via various advanced character recognition algorithms
**4)	Guided Translation:** To make the resource accessible to an international audience of both scholars and laymen, it is important for the information to be translated into various languages. As context is critical for accurate translation, this can be done with a guided machine learning algorithm, which can intake manually translated sample pages as its training data.

## Presentation and Accessibility of Data:
To make the extracted data as useful as possible, it is critical to present it in intuitive and simple formats. This is where visualization of the data could play a large role. Although there are other exceptional expenses included in the data, most of it the expense information involves seating prices and the number of tickets sold. Additionally, the date and play performed are two critical and consistent, extractable datasets.

One intuitive visualization method could utilize a seating map (similar to ones used by Ticketmaster etc.) for the CF Theater as its basis. The user could select to scroll through two distinct data sets over the span of 113 years with a granularity down to single days: (1) seating prices (2) attendance, both based on different parts of the theater. In addition to access to numerical values via mouse-overs, the data can be visualized with a color/heat map, with a corresponding legend.

Another mouse-over for the stage could lead to a hyperlink giving a brief overview for the play (potentially even incorporating defining clips from contemporary renditions) for the corresponding date. This will help the user link the content and context of the performed play with attendance numbers and ticket pricings via visual observation.

Additionally, the option of averaging or data summaries for longer time spans would be very critical to make broader observations compared to just individual dates. Options like averaging attendance and price values per play (over its complete show dates), summarizing attendance trends based on certain blocks (e.g. the premier lodges) can be automated outputs that facilitate interpretation of the data. Since flexibility in use is crucial for this tool to be beneficial for the scholar community, summaries based on user-defined constraints would also be a critical feature to incorporate.

## Audience:
This format of visualization is primarily intended for scholars interested in extracting information relating to the theater. It intends to maximize flexibility of data analysis by incorporating features that allow the user to customize the span of the displayed data. However, the visual nature of the tool, in addition to its availability in various languages, makes it accessible to a broader audience, including younger students or theater history enthusiasts.


