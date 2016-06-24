---
layout: post
title:  "Anaphora Resolution"
date:   2015-12-17
categories: Natural-Language-Processing

---

Natural Language Processing aims at designing and building softwares that can analyze, understand, and generate human languages, so that eventually humans will be able to communicate with the machines using natural languages. NLP works at the intersection of  computer science, artificial intelligence, and computational linguistics. Processing or understanding of human languages, especially written texts, requires analysis and implementation at different linguistic levels such as Part-of-Speech tagging at word level;  syntactic parsing at the sentence or structural level; semantic analysis at the level of meaning and finally discourse analysis at the discourse or text level. Resolving anaphora is another prime task in this field.

Reference to an entity that has previously been used in a discourse is known as anaphora. Anaphora resolution is the process of identifying the referent of the referred expression. The resolution requires much attention in case of Hindi language. The motivation of anaphora resolution in case of Hindi language comes from its real time applications in NLP which involves offline question answering, information extraction, automatic summarization, machine translation. 

The work that I am upto these days is based on the examination and development of assets which could be utilized for anaphora resolution in Hindi language and exploration of linguistic features to be useful in the resolution process. The algorithm is based on Mitkov's knowledge poor approach which does not rely on linguistic and domain knowledge, work even without parsing and employs AI techniques like neural networks, situation semantic framework etc.

First, the annotated input text is created using syntactic constraints like gender agreement, number agreement, honorifics and then the incorrect expressions are eliminated out after comparing. The remaining candidates are compared based on the score assigned to each candidate.
Scoring scheme as well as some of the indicators used are specifically drawn for Hindi language. The highest scored NP(Noun Phrase) in the set of potential candidates is finally chosen as the antecedent. In a tie case, the closest candidate to the anaphora is chosen instead. 

From the results, one could observe that a high accuracy resolution is attained by using simple and easy to understand text than the one involving complex co-reference relations.



_______________________________________________________________________________________________________________________________________________________



