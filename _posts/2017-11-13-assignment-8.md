---
layout: post
published: true
category: commentary
title: Assignment 8
author: Parker
---
### Alien Reading Commentary

As someone who has had a decent amount of experience in natural language processing (I took 6.864 last year), I found the article pretty interesting overall, but there were some points that could have been improved upon. Particuarly, I agree with his argument that its important to separate the computer's understanding of natural language with our own; however, there has been extensive progress in computer representation of language in recent years, especially with deep neural models. The author misrepresented a computer's ability to produce a coherent sentence by choosing to include a piece generated from a Markov chain model, an algorithm which is nearly 30 years old, rather than including text generated from a more recent breakthrough.

While these tools aren't perfect for studying humanities as they currently are (nor will they ever be), we may still use them as long as we make sure to note that as powerful as they are, they are also limited in many ways.

### Working With Stanford NER

I chose to work with the Stanford NER by interfacing with it using Python nltk. It was overall pretty easy to get it working, it just required installing Python nltk and downloading the appropriated JAR files for the Stanford NER. I have reproduced the script below.


    from nltk.tag.stanford import StanfordNERTagger

    CLASSIFIER = `classifiers/english.all.3class.distsim.crf.ser.gz`
    JAR_FILE = `stanford-ner.jar`

    def extract_ner(filename):
        st = StanfordNERTagger(CLASSIFIER, JAR_FILE)
        file_text = ``
        with open(filename) as f:
            for line in f:
                file_text += line
            return st.tag(file_text.split())

    if __name__ == `__main__`:
        ner = extract_ner(`ulysses.txt`)
        print(ner)
        for word, tag in ner:
            if tag != `O`:
                print(word, tag)
                
I tried the Stanford NER on a few poems ("Ulysses" by Tennyson, "Because I Could Not Stop for Death" by Dickenson) but the algorithm unfortunately could not find any named entities. When I tried it on Frederick Douglass' essay "John Brown," it performed much better, suggesting that the Stanford NER is unable to perform well on poetry, but excels at understanding prose.
           