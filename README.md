# Hate-speech-detection
This project is an approach of detecting tweeter hate speech using basic NLP features.  Hate speech detection comes under the domain of Sentiment Analysis of Natural Language Processing. The goal of this project is to get text classification model building process.

The dataset is from the link below:
https://datahack.analyticsvidhya.com/contest/practice-problem-twitter-sentiment-analysis/

The data has 3 columns id, label, and tweet. label is the binary target variable and tweet contains the tweets 

The following are the steps performed:
## 1) Pre-processing or Text Cleaning
This is the step of removing noise from the data such as the ‘hash’ tag (‘#’) and Unicode characters that look like foreign non-English letters.
## 2) Features Engineering
It performs the task of keeping only useful information from the content. The unnecessary contents removed are:
*	Stop words removal
*	Negative words detection (like no, not, etc.)
*	Check for the presence of 100 rare words.
*	Check for prompt words like when, what, how, who , whom, why, etc.
*	Check for the 20 most common words.
## 3) Train a Machine Learning model for classification
In this step, the data is divided into 80% training set and 20% test set to evaluate the model created on unseen instances. Logistic Regression from 'sklearn'  is used for classification since the task consists of Binary Classification (Hate speech (1) or not(0)).
## 4) Evaluate the ML model
The last step is the evaluation of the model on unseen data to check the accuracy.
>python HateSpeechDetection.py
