# 2020-presidential-topics
A visualization of topics for the 2020 election

### Visualizations

For the interactive visualizations the team used Tableau and published various datasets for sentiment analysis determined using VADER Sentiment Analysis package. These visualizations include sentiment distribution counts between Trump and Biden, time series, as well as a smaller dataset for a location map of tweets from different states.

The distribution of sentiments are shown in the histogram chart and box plot with the time series shown in the line graph. The location map shows average sentiment scores for each state leading up to the election.

Description: Tableau was utilized for our visualization assessments. Tableau is an interactive data visualization software that is widely used across industry. The data generated from the sentiment analysis code above was exported to a pkl or xlsx file to be uploaded and manipulated in tableau.

Installation: There are multiple versions of tableau that can be used for this dataset. The team used tableau desktop, since it was available at no additional cost through the CSE 6242 course at Georgia Tech. Tableau desktop is the only required software to run this visualization. 

Execution: After installing tableau, export the sentiment analysis data into an xlsx or pkl file for review. Once you have the sentiment_df.xlsx file exported and saved, then you will be able to create a connection to upload. Click on the bottom data source tab and select the connect “to a file: Microsoft Excel.” The query will execute, and your tabulated data will be shown in sheet 1 after updating the data. Next, visualizations can be made via the sheets tab and placing different attributes into the dimensions and measure groupings. In order for ease of execution, the team has compiled all data sets and the final dashboards/sheets into one simplified tableau file. This can be found by opening the “Sentiment Tableau.twb” file. All sheets and dashboards are auto populated after opening this file in Tableau.

### Topic Modeling

For topic modeling analysis the team used various Python packages including Gensim, NLTK, and Spacy to find which works best for cleaning and generating word clouds for undiscovered topics. The notebooks for LDA Analysis show word cloud generation from tweets analyzed from a MongoDB Cluster.

The tweets were gathered and saved using Node Red's free Twitter API from the weeks leading up to the U.S. Presidential Election for 2020. Using the LDA Analysis notebook the user can view and generate word clouds which contain topics discussed by users.

Installation:
- Anaconda: https://docs.anaconda.com/anaconda/install/
- `conda env create -f environment.yml`

Execution (Demo):
- `conda activate new_env`
- `jupyter-lab`
- Run LDA-Analysis-Demo.ipynb for topic modeling analysis


### Sentiment Analysis 

Description:
The team used the NLTK package specifically nltk.sentiment.vader to import the “SentimentIntensityAnalyzer” model.  VADER stands for Valence Aware Dictionary for Sentiment Reasoning as it can determine the polarity and intensity of unlabeled text data. This model uses a gold standard sentiment lexicon dictionary that will map the text to its emotion intensity based on human-annotated labels.

The VADER SentimentIntensityAnalyzer is ideal for social media texts since it can interpret the intensity of the texts from capitalization, emoticons, and punctuations. It was determined to be the most optimal model for analyzing tweets.

The model will determine a positive, negative, neutral, and compound score. The overall polarity score used is the compound score, which is determined by Vader's normalization equation and will be on a scale from -1 to 1.

Installation:
I used an older version of Python to perform my analysis. I would advise installing Python 3.5.6 and Anaconda (https://www.anaconda.com/products/individual). 

To install the nltk library run: 
conda install -c anaconda nltk

Execution:
After loading the Sentiment Analysis.ipynb jupyter notebook you will find multiple packages, libraries, and functions to install. I would recommend using Anaconda for all its installation. Next run each cell to retrieve the data, pre-process the text, and finally run the sentiment analysis model. Read the comments on each cell for guidance.
