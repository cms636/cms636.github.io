---
layout: post
published: true
category: updates
title: The Perils of Omeka
author: 'Xinwen Liu, Peter Downs'
---
## The Perils of Omeka

With so many photos to pick from, there were many possible narratives. We decided to try to tell a story involving women: in the public realm, of different classes, in relationship to public space. We narrowed our focus to show all of the way that women subvert the idea of "nobility", through action, dress, or role. You can [view the Omeka collection here](http://peterxinwen.omeka.net/collections/show/1).

As you may be able to tell from our final result, we had lots of troubel using Omeka to this end. I have  rarely used less-friendly software. The curation process went something like this:

1. Browse the photo `.jpg` files, and assemble a collection of files by copying the relevant images into a separate folder. Omeka fails to provide any tools for performing this act of curation, only listing and displaying previously-curated images.

2. Create a new `.csv` file containing only the metadata relevant to these photos, by searching through the full data set for one row at a time.

3. Write code to convert the `.csv` file encoding from `WINDOWS 1252` to `UTF-8` so that Omeka would properly render non-US characters with accents.

4. Manually upload images for each of the items that Omeka was able to import from the `.csv` file.

5. Repeat all of these steps because we changed our curation concept to the one described above. Give up halfway through because it's a waste of time.

Omeka does a terrible job of generating interesting, useful, websites. It is impossible to dictate the order of the items in the display of a collection. There is no full-screen image viewer. The output website is bland and difficult to theme. The importing options are rigid and badly explained. All in all although we felt that curation is worth practicing and an interesting academic and practical subject, Omeka was a bad tool to use given the difficulty involved.
