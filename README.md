# 2020-presidential-topics
A visualization of topics for the 2020 election

### Visualizations

For the interactive visualizations the team used Tableau and published various datasets for sentiment analysis determined using VADER Sentiment Analysis package. These visualizations include sentiment distribution counts between Trump and Biden, time series, as well as a smaller dataset for a location map of tweets from different states.

The distribution of sentiments are shown in the histogram chart and box plot with the time series shown in the line graph. The location map shows average sentiment scores for each state leading up to the election.

Installation:
- Install Tableau Desktop https://www.tableau.com/products/desktop/download

Execution (Demo)
- Open .twb file and set data source to data defined via project via sentiment_df.xlsx

Published interactive visualizations:
- Time Series: https://public.tableau.com/profile/rapid.dev#!/vizhome/SentimentTableau/Dashboard4
- Distribution Scores: https://public.tableau.com/profile/rapid.dev#!/vizhome/Trumpvs_BidenSentimentDistribution/Dashboard1
- Location Sentiment: https://public.tableau.com/profile/rapid.dev#!/vizhome/Trumpvs_BidenSentimentMap/Dashboard2

### Topic Modeling

For topic modeling analysis the team used various Python packages including Gensim, NLTK, and Spacy to find which works best for cleaning and generating word clouds for undiscovered topics. The notebooks for LDA Analysis show word cloud generation from tweets analyzed from a MongoDB Cluster.

The tweets were gathered and saved using Node Red's free Twitter API from the weeks leading up to the U.S. Presidential Election for 2020. Using the LDA Analysis notebook the user can view and generate word clouds which contain topics discussed by users.

Installation:
- Anaconda: https://docs.anaconda.com/anaconda/install/
- `conda env create -f environment.yml`

Execution (Demo):
- `conda activate new_env`
- `jupyter-lab`
- Authenticate via Kaggle: Go to https://www.kaggle.com/ and sign in
- Under profile picture -> my account -> account settings -> Create API Token
- Update kaggle.json token file to be in your home directory (for Linux users ~/.kaggle/kaggle.json or C:\Users<Windows-username>.kaggle\kaggle.json on Windows)
- Run LDA-Analysis-Demo.ipynb for topic modeling analysis


### Sentiment Analysis 

Description:
The team used the NLTK package specifically nltk.sentiment.vader to import the “SentimentIntensityAnalyzer” model.  VADER stands for Valence Aware Dictionary for Sentiment Reasoning as it can determine the polarity and intensity of unlabeled text data. This model uses a gold standard sentiment lexicon dictionary that will map the text to its emotion intensity based on human-annotated labels.

The VADER SentimentIntensityAnalyzer is ideal for social media texts since it can interpret the intensity of the texts from capitalization, emoticons, and punctuations. It was determined to be the most optimal model for analyzing tweets.

The model will determine a positive, negative, neutral, and compound score. The overall polarity score used is the compound score, which is determined by Vader's normalization equation and will be on a scale from -1 to 1.

Installation:
- Anaconda: https://docs.anaconda.com/anaconda/install/
- `conda env create -f environment.yml`

Execution (Demo):
- `conda activate new_env`
- `jupyter-lab`
- Authenticate via Kaggle: Go to https://www.kaggle.com/ and sign in
- Under profile picture -> my account -> account settings -> Create API Token
- Update kaggle.json token file to be in your home directory (for Linux users ~/.kaggle/kaggle.json or C:\Users<Windows-username>.kaggle\kaggle.json on Windows)
- Run LDA-Analysis-Demo.ipynb for topic modeling analysis
