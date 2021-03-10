---
layout: post
title: Natural Language Understanding - Information Extraction, Store, Retrieval and Inference  
date: '2021-03-10T14:31:00+00:00'
tags:   AI ML NLU
---

Natural Lanugage Understanding has revived and progressed significantly in last 10 years applying Deep Learning techniques. With success of GPT-3 announced last year (and constant improvements of BERT models) multiple experimentatal business use cases are being pursued in Industry. But, a full-fledged industry use-case in any specific or narrow domain is still elusive. Here is a quick summary of challenges, current solution and opportunities.

<h2> Information Extraction </h2> <br>
<b>Opportunities:</b>
The OCRs have seen wide adoption with increase in accuracy of extraction in recent times using DL techniques. With majority of the contents are in digital format, sevaral businesses are building crawlers to source, parse and filter relevant data. 
The biggest opportunity here will be in building domain specific corpus and knowledge base with high accuracy and low bias.
<b>Challenges:</b>
Trust in the content that is published is a key challenge faced across industry. There is no mechanism to verify a trustworthy source at the moment and most of it is entrusted in the big-brands.
Transparency & Privacy balance is critical as well, as majority of curated content are paid for and not freely accessible for building models.
<b>Current Solution & Algorithms</b>
Current solution for information extractions are OCR, Crawlers and ML based parsers. The computer vision CNN algorithms are used predominatly in the OCRs, while RNN, LSTMs and Transformers are used for langauge parsing and extractions. The process involves tokenization, annotations, tagging, parsing, feature selection, etc to extract the right entities and relationsips. 
Datasets: Refer Information Representation & Storage.

<h2> Information Representation & Storage </h2> <br>
<b>Opportunities:</b>
Domain specific knowledge representation and curation of corpus and knowledge base. 
<b>Challenges:</b>
The continuous building of domain specific Corpus and Knowledge base is core to NLU engines. The inputs in and out of context sentences and the output that could result in single or mutiple relations presents an issue in learning. 
The linking of corpus and KB along with negative data sets and its classification are other key challenges. 
The solutions for information extraction and parsing influences the quality of representation and storage. 
<b>Current Solution & Algorithms</b>
Vector Space Models are used widely to store and represent entities. These models go through process of defining right matrix, weighting the models (Normalization, TF-IDF, PMIs) Dimensionality reduction (LSA, LDA, PCA, Autoencoders,) and models for vecot comparisions (L2 norms, Cosine, Dice, Jaccard, KL etc). The most popular ones that are used for Reighweighting and dimensionality reductions are Word2Vec, and Glove models. The core IT tools used for storing entity and relationships with Graph DB suche as neo4J.
Sentences are represented and stored in a Tree based network.
Other representation models that are emerging includes Word embeddings, Directional bag-of-words, POS tags, N-Grams, Wordnet Synets, entity mentions, etc. 
The models used here to help with learning relationships include FF NN, SVM, LSTM and Transformers. 
The evaluation of the models with precision, recall, F-statistic, microveraging (equal weightage to problem instance) and macroaveraging (equal weightage to relations) requires balanced judgement.
Datasets: Wikilinks Corpus, freebase (stopped in 2017)

<h2> Information Retrieval </h2> <br>
<b>Opportunities:</b>
1. Query systems using Natural Language. The 
2. Q&A based Chatbot Systems for user interactions. The Customer Service products have already adopted the solution, with wider and deeper application in future. 
<b>Challenges:</b>
For many years search engines and opensource tools such as Apache Lucene has provided indexing, search and sorting algorithms to provide results. Most, of these relied on Regular Expression inputs to fetch relevant outputs. 
The solutions in this domain are dependent on Information extraction, representation and storage evolution.
<b>Current Solutions & Algoritms</b>
GraphDBs are  accessed with Gremlin/SPARQL, Cyphers. Most of the information retrieval is pulling data from files ausing tools like elastic search or file operation and storing in memory for operations. 
Datasets: SQUaD


<h2> Inference </h2> <br>
<b>Opportunities:</b>
Paraphrasing the text in multiple-structures is key to aiding human understanding of complex domains. This coupled with summarization of information from structured and unstructured content has use-cases across industry domains. Another, widely used model is the CRM domain is sentiment analysis. 
<b>Challenges:</b>
Availability of datasets that could helps in building strong inference engines. 
<b>Current Solution:</b>
Sentence encoders, RNN, Attention based RNN, Transformers and LSTMs to infer the relationship between sentences. 
Datasets: Penn Paraphras, DNC, GLUE, NLI Style fever, SciTail, MultiNLI, SNLI
Sentiment Datasets: IMDB, Lillian Lee Group, Amazon Customer reviews, sentiment and social networks, SST, Opinion Lexicon, SentiWordNet, Harvard General Inquirer, SocialSent, LIWC.


Some great use cases are in experimental stages in each of the above domain. Its exciting times to apply current techniques to solve simple problems. As always, startups are in the fore-front of these technologies, while hyperscalars are working towards democratizing these technologies for businesses.