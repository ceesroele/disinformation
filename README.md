# Disinformation: articles and notebooks based on data from EUvsDisinfo

> Different notebooks to support articles I published at Medium

## Disinformation Topics over Time

> Goal: model topics in the EUvsDisinfo database and track them over time

I created a dataset based on the scraped content of the EUvsDisinfo database which has over 14,000 reports on "disinformation cases". Assuming that each report refers to one topic, I used BERTopic to model the topics, and created different views on the data.

Most important outcomes:

* Creation of a list of topics characterised by their prevalent terms. Based on domain knowledge, I think this list is realistic
* Pinpointed which is the most representative article in the entire database
* Innovatively used pandas to visualise the terms for each topic in a matrix with their scores encoded by the intensity of colour
* Displayed the topics in a hierarchy to demonstrate their relations of similarity
* Visualised different topics over time, with the selection of what topics to visualise based on three approaches 

Article:
[Disinformation Topics over Time](https://medium.com/p/5c9ec21300f9)

Notebook:
[Disinformation Topics over Time](https://github.com/ceesroele/disinformation/blob/main/DisinformationTopicsOverTime.ipynb) 


## An exploration of the notion of "disinformation" as used in the EUvsDisinfo website

> Goal: Make sense of the actual usage of the word "disinformation"

Based on the scraped content of the website [EUvsDisinfo](http://euvsdisinfo.eu/) I created a dataset of all sentences
containing the word "disinformation".

Most important outcomes:

* The usage of "disinformation" is strongly correlated with the notion of "narrative"
* We determined a number of KMeans based clusters to allocate the different sentences to 
* The _centroids_ of the clusters are the most important terms of each cluster, so they give an impression of what 
the clusters are about.
* By combining the top terms of clusters with their Part-of-Sentence roles, we get to topic modelling beyond listing terms and gain some insight in the basis of the narratives by identifying places, common names, and verbs.

Article:
[Exploring “disinformation” at EUvsDisinfo](https://medium.com/p/6cec6c7f05e2)

Notebook:
[Exploring "Disinformation" at EUvsDisinfo](disinformation.ipynb)
