# 2020-presidential-topics
A visualization of topics for the 2020 election





## Sentiment Analysis README

Description:
The team used the NLTK package specifically nltk.sentiment.vader to import the “SentimentIntensityAnalyzer” model.  VADER stands for Valence Aware Dictionary for Sentiment Reasoning as it can determine the polarity and intensity of unlabeled text data. This model uses a gold standard sentiment lexicon dictionary that will map the text to its emotion intensity based on human-annotated labels.

The VADER SentimentIntensityAnalyzer is ideal for social media texts since it can interpret the intensity of the texts from capitalization, emoticons, and punctuations. It was determined to be the most optimal model for analyzing tweets.

The model will determine a positive, negative, neutral, and compound score. The overall polarity score used is the compound score, which is determined by Vader's normalization equation and will be on a scale from -1 to 1.

Installation:
I used an older version of Python to perform my analysis. I would advise installing Python 3.5.6 and Anaconda (https://www.anaconda.com/products/individual). 

To install the nltk library run: 
conda install -c anaconda nltk

Execution:
After loading the Sentiment Analysis.ipynb jupyter notebook and installing the required packages, libraries, and functions, run each cell to retrieve the data, pre-process the text, and finally run the sentiment analysis model.
