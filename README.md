## What Do We Know about Business Insight with COVID-19 Open Research Dataset?--- LDA Topic Modeling 
***
A blog describing this project is available at: 
https://leizhipeng.medium.com/topic-modeling-of-covid-19-open-research-dataset-7474710bfbce
***
### CONTENTS
* Introduction
* Dataset
* Data pipeline
* Word Cloud
* Visualization of Topics
***
### Introduction
Since the COVID-19 pandemic, academic society has published many papers about COVID-19, SARS-CoV-2, and related coronaviruses. 

I use the latent Dirichlet allocation (LDA), a popular text mining method for topic modeling, to find business insight in a dataset of COVID-19 publications. 

I am trying to answer the following questions.
* What do we know about business topics associate with COVID-19? 
* What has been published about information sharing and management?
* What has been published about social science that may impact business? 
* What do we know about the topics that combine business and health care, or social science and health care?


### Dataset 
The dataset is downloaded from [COVID-19 Open Research Dataset Challenge](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge).

While the dataset has information and full text for each paper, I only mine the abstracts in order to simplify the task. The abstracts are in the dataset file “metadata.csv” downloaded on November 9th, 2020.

### Data pipeline
In the data pipeline, the raw text data is imported from a CSV file and is preprocessed using RegEx and other normalization skills. I use Pandas framework to manage the data and use Gensim framework to handle natural language processing and create an LDA model for generate topics. I use Word Clouds and pyLDAvis packages to visualize the topics.  
![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/figures/pipeline.png?raw=true)

### Word clouds
The word cloud plots terms appearing in all documents. The general theme of the dataset is medical research on coronavirus. The high-frequency terms are study, disease, study, effect, approach, infect, and etc.
![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/figures/word_cloud.png?raw=true)

 



