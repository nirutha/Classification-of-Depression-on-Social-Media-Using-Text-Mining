---
jupyter:
  jupytext:
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.2'
      jupytext_version: 1.7.1
  kernelspec:
    display_name: Python 3
    language: python
    name: python3
---

# Impact of pandemic on mental health using twitter data


### The goal of this project is to analyze the impact of the pandemic on mental health and the different reasons of pandemic people are suffering.



### We perform data collection using the tweepy module, pre-processing of the tweet data and sentiment analysis using the textblob module for depression analysis.


### We train a model for processed tweets data using different classifiers to predict the tweets as depressed or non-depressed. The depressed tweets are used to further train a model to categorize into different groups based on the most common reasons of pandemic using clustering algorithms.


### The machine learning algorithms of classification and clustering are verified and evaluated based on corresponding metric methods for analysis. 


### Requirements:
    * Python 3.6.1 or Higher
    * Twitter developer account
    * A bunch of modules (Keras, TF, Numpy, Sklearn, Pandas, Itertools)
    


### Code folder contains the scripts Depression_sentiment_analysis.ipynb and Clustering.ipynb 


### Data folder contains csv files collected from twitter api for tweets data


### Input folder contains the oauth csv file which has tweets access token and secret and API access token and secret


### Input folder also contains combined.csv file which is created by combining and consolidating all the collected tweets into a single csv


### Steps:
    * Create a twitter developer account and get token values for accessing the twitter API.
    * Import the required modules to create the environment.
    * Run data collection function in Depression_sentiment_analysis.ipynb to obtain the tweets data.
    * Run pre-processing step to remove url, punctuations, stop words and tokenize the words with lemmatization and stemming.
    * Run the sentiment analysis step to classify the data into positive, negative and neutral tweets based on the depression dictionary called dictionary.tsv
    * Run the classification modeling step to predict the tweet data as depressed or non-depressed using Naive-bayes, logistic regression, Decision tree, random forest, svm and neural network classifiers. 
    * Run the evaluation step containing evaluateMyModels() function to analyze the performance metrics of each classifiers.
    * Run the Clustering.ipynb script for performing k-means clustering on the processed data with visualization of the clusters. 
    




```python

```
