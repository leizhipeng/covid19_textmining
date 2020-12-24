## What Do We Know about Business Insight with COVID-19 Open Research Dataset?--- LDA Topic Modeling 
***
* This is a project for Udacity's data science nanoprogram. 
* A blog describing this project is available at: 
https://leizhipeng.medium.com/topic-modeling-of-covid-19-open-research-dataset-7474710bfbce
***
### CONTENTS
* Introduction
* Dataset
* Data pipeline
* Word Cloud
* Visualization of Topics
* Next step

***
### Introduction
Since the COVID-19 pandemic, academic society has published many papers about COVID-19, SARS-CoV-2, and related coronaviruses. 

I use the latent Dirichlet allocation (LDA), a popular text mining method for topic modeling, to find business insight in a dataset of COVID-19 publications. 

I am trying to answer the following questions.
* What do we know about business topics associate with COVID-19? 
* What has been published about information sharing and management?
* What has been published about social science that may impact business? 
* What do we know about the topics that combine business and health care, or social science and health care?


***
### Dataset 
The dataset is downloaded from [COVID-19 Open Research Dataset Challenge](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge).

While the dataset has information and full text for each paper, I only mine the abstracts in order to simplify the task. The abstracts are in the dataset file “metadata.csv” downloaded on November 9th, 2020.

***
### Data pipeline
In the data pipeline, the raw text data is imported from a CSV file and is preprocessed using RegEx and other normalization skills. I use Pandas framework to manage the data and use Gensim framework to handle natural language processing and create an LDA model for generate topics. I use Word Clouds and pyLDAvis packages to visualize the topics.  
![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/figures/pipeline.png?raw=true)

***
### Word clouds
The word cloud plots terms appearing in all documents. The general theme of the dataset is medical research on coronavirus. The high-frequency terms are study, disease, study, effect, approach, infect, and etc.
  ![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/figures/word_cloud.png?raw=true)

***
### Visualization of Topics
Topics related to business are determined using LDA topic modeling. 
#### Economic Crisis
COVID-19 causes a significant backward in the economy, especially on food supplies.

  ![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/figures/economy.png?raw=true)
  
#### Social Media
The online discussion on COVID-19 has distinct temporal and topical trends. 

  ![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/figures/social_media.png?raw=true)

#### School Closure
Necessary measures are needed to prevent the virus's spreading inside schools. 

  ![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/figures/school_closure.png?raw=true)

#### Video on Influenza
YouTube has a huge increase of viewership during the COVID-19 outbreak but with misleading videos prevailing and medical content from WHO underrepresented. 

  ![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/figures/video.png?raw=true)

#### Mental Health
The anxiety and depression symptoms among healthcare workers are high under the COVID-19 outbreaks. Can we lessen the stress through business measures? 

  ![alt text](https://github.com/leizhipeng/covid19_textmining/blob/main/figures/depression.png?raw=true)

***
### Next Step
I will introduce Bert for sentence embedding vector in the topic modeling.