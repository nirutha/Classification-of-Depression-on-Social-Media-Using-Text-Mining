{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Impact of pandemic on mental health using twitter data"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### The goal of this project is to analyze the impact of the pandemic on mental health and the different reasons of pandemic people are suffering. \n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### We perform data collection using the tweepy module, pre-processing of the tweet data and sentiment analysis using the textblob module for depression analysis."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### We train a model for processed tweets data using different classifiers to predict the tweets as depressed or non-depressed. The depressed tweets are used to further train a model to categorize into different groups based on the most common reasons of pandemic using clustering algorithms."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### The machine learning algorithms of classification and clustering are verified and evaluated based on corresponding metric methods for analysis. "
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Requirements:\n",
    "    * Python 3.6.1 or Higher\n",
    "    * Twitter developer account\n",
    "    * A bunch of modules (Keras, TF, Numpy, Sklearn, Pandas, Itertools)\n",
    "    "
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Code folder contains the scripts Depression_sentiment_analysis.ipynb and Clustering.ipynb "
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Data folder contains csv files collected from twitter api for tweets data"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Input folder contains the oauth csv file which has tweets access token and secret and API access token and secret"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Input folder also contains combined.csv file which is created by combining and consolidating all the collected tweets into a single csv"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### output folder which saves the graphs and output images"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Steps:\n",
    "    * Create a twitter developer account and get token values for accessing the twitter API.\n",
    "    * Import the required modules to create the environment.\n",
    "    * Run data collection function in Depression_sentiment_analysis.ipynb to obtain the tweets data.\n",
    "    * Run pre-processing step to remove url, punctuations, stop words and tokenize the words with lemmatization and stemming.\n",
    "    * Run the sentiment analysis step to classify the data into positive, negative and neutral tweets based on the depression dictionary called dictionary.tsv\n",
    "    * Run the classification modeling step to predict the tweet data as depressed or non-depressed using Naive-bayes, logistic regression, Decision tree, random forest, svm and neural network classifiers. \n",
    "    * Run the evaluation step containing evaluateMyModels() function to analyze the performance metrics of each classifiers.\n",
    "    * Run the Clustering.ipynb script for performing k-means clustering on the processed data with visualization of the clusters. \n",
    "    "
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.8.6"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 4
}
