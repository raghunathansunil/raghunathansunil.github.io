---
layout: post
title: Chatbot Architecture & techniques used in all non-mission critical chatbots
  .
date: '2020-07-15T17:25:00+00:00'
tags: Chatbot
---

There are two broad architecture & techniques for chatbots in industry: 
1. Q&A based pioneered by DeepQA research in IBM Jeopardy game. WeChat uses this for service tasks, Information, Knowledge.  (Covered here)
2. AI/ML engines using techniques: RNN, AR resolution, ANN, handling response diversity in a dialogue. 
 
Q&A Ontology: Jeopardy 2011 USD 1m win based on IBM Watson DeepQA engine. The award winning Q&A/Ontology based engine is built on Apache UIMA-AS framework & Hadoop. This involved perfecting Q&A models and techniques to improve Speed - < 3 sec response, Precision (correct Answer) 85% and above, confidence (for Buzz-in) 70% and above, complex language processing and collation of wide breadth KB.  The core approach:
a. ongoing content acquisition, 
b. Question Analysis: classification, LAT/relation detection & decomposition 
c. massive parallel processing, multi-expert activities: hypothesis generation, filtering, evidence scoring, 
d. synthesis of output by merging & ranking, 
e. ranking estimation and result.
Complex Stochastic and Optimization techniques drive wagering strategy for category selection, Buzz-ins, & double/final Jeopardy wagering.

https://www.aaai.org/Magazine/Watson/watson.php
