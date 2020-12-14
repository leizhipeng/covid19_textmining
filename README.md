# Topic Modeling of COVID-19 Open Research Dataset

***
A blog describing this project is available at: 
https://leizhipeng.medium.com/topic-modeling-of-covid-19-open-research-dataset-7474710bfbce


## Purpose
Finding latent topics for publications on COVID-19 

## Background
Since the COVID-19 pandemic, academic society has published many papers about COVID-19, SARS-CoV-2, and related coronaviruses. 
How can we efficiently find useful information among these papers? 
As the COVID-19 pandemic involves many disciplines, it would be urgent to classify the literature into different groups according to topics. However, the topics are unsupervised variables. 
Can machine learning methods find the latent topics for publications on COVID-19?
I use the latent Dirichlet allocation (LDA), a generative statistical model in natural language processing, to explore many COVID-19 texts and create groups according to data similarity.

## Dataset 
The dataset is downloaded from [COVID-19 Open Research Dataset Challenge](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge).

While the dataset has information and full text for each paper, I only mine the abstracts in order to simplify the task. The abstracts are in the dataset file “metadata.csv” downloaded on November 9th, 2020.

## Data pipeline
![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/pipeline.png?raw=true)

## Word clouds of topics
![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/wordclouds.png?raw=true)

 



