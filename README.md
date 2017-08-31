# Enron - Search for sensitive information

Enron email dataset was used to understand the nature of false positives in a proprietary software system which was capable of recognizing personally identifiable information present in email data.The proprietary system tagged emails  based on complex set of rules and regular expression matches.However, the system had lots of false positives.

They wanted to build a supervised machine learning model that can categorize emails more accurately. The major issue here was to identify  postive samples that contain PII information. Hence we devised a methodology to intelligently identify sub groups of emails based on the lingusitic information so that it can be used to extract samples(positve) which can be used to develop supervised machine learning models.

* Data Description : Meta data about each email was present in the form of raw text files along with tag information.   

* Goal: The goal of the project was to identify sub groups of email data that are probable candidates for true positives  

* Model :Word2vec is a group of related models that are used to produce word embeddings. These models are shallow, two-layer neural networks that are trained to reconstruct linguistic contexts of words. Word2vec takes as its input a large corpus of text and produces a vector space, typically of several hundred dimensions, with each unique word in the corpus being assigned a corresponding vector in the space. Word vectors are positioned in the vector space such that words that share common contexts in the corpus are located in close proximity to one another in the space [Wikipedia]  

* Results:  Five prominent Clusters of data were identified using the Word2Vec Model.