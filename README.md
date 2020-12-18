### NLP_Homework


### Student: Michael De Paula



<p align="center">
    <ins><b>Natural Language Processing (NLP):</b><br><ins>
    
</p>

Within this repository you will find a Jupyter Notebook file that contains code for natural language processing.  Using code we will import articles related to cryptocurrencies, specifically Bitcoin and Ethereum. The articles we are pulling are coming from NewsAPI. Once the articles are pulled we are going to collect the articles and code them into a sentiment analysis in a dataframe. We will then describe the sentiment analysis and make a decision on which coin had the highest mean positive score, highest compound score and highest positive score. 

We will continue coding with tokenization using nltk imports. With tokenization we will first clean out the most common stopwords in the english language. We will also create a function that creates a list of words, sets stopwords, makes everything lower case, separates puntuation and lemmatizes the words into root words for the texts in each of the articles in the datatframe. The result of this function will also be included in the dataframe under a column of the same name. 

Next we will create a frequency analysis using ngrams. This frequency analysis helps us identify the frequently used words using counter functions and the ngrams import. In order to identify frequency we will be using a comprehensive loop as well as function that helps us identity the word counts. With this word count we will be creating a Word Cloud and visualizing the frequently used words with the most frequently used being displayed larger. To do this we used matplotlib.

Finally, we will code Named Entity Recognition (NER) which will tag specific words within each of the articles. Here we will create a for loop that converts a list to a string in order to pull the articles using a variable and display the tagged text. This tagged text is a visualization of all the combined articles that were pulled early in the notebook. 

__Imports used:__  

- import os
- import pandas as pd
- from newsapi import NewsApiClient
- from dotenv import load_dotenv
- from nltk.sentiment.vader import SentimentIntensityAnalyzer
- analyzer = SentimentIntensityAnalyzer()
- %matplotlib inline
- from nltk.tokenize import word_tokenize, sent_tokenize
- from nltk.corpus import stopwords
- from nltk.stem import WordNetLemmatizer, PorterStemmer
- from string import punctuation
- import nltk
- nltk.download('stopwords')
- nltk.download('punkt')
- import re
- from collections import Counter
- from nltk import ngrams
- import matplotlib as mpl
- from wordcloud import WordCloud
- import matplotlib.pyplot as plt
- plt.style.use('seaborn-whitegrid')
- import spacy
- from spacy import displacy
