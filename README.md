# Using Natural Language Processing on Spotify 2019 Top Artists
This project was inspired by Spotify's user recap. I wanted to practice NLP techiques on the most popular artists of 2019. 

This project analyzes the following albums: 
    1. WHEN WE FALL ASLEEP, WHERE DO WE GO? - Billie Eilish (2019)
    2. Hollywood’s Bleeding - Post Malone (2019)
    3. Thank u, next - Ariana Grande (2019)
    4. Care Package - Drake (2019)

## Getting started:
Before web scraping anything from the Genius website, you must create an account as an API client which will provide you with a client_id and client_secret which will later get you started with the site’s web scraping process. The Genius API documentation is available at https://docs.genius.com/. 

The function that scrapes each album is available in the albumscraper.ipynb Jupyter Notebook. **I created a file called settings.py which contained my access_token** that I recieved when creating my Genius API client account. I called this file in the notebook to access Genius' API. 

## Artist EDA Methods:
In the 02_eda folder, you can find a jupyter notebook with the following EDA methods for each artist/album:
 - Cleaning Lyrics Dataframe
 - Analyzing word count + unique word count of songs
 - nltk.sentiment SentimentIntensityAnalyzer library usage
 - Most Common Terms used in songs (using sklearn.feature_extraction CountVectorizer and Tfidf Vectorizer)
 - Topic Modeling using sklearn.decomposition LatentDirichletAllocation library
 
 ## Media Folder:
 The media folder contains: (1)matplotlib sentiment analysis graph for each album (2)common term analysis for each album (3) 2 tableu charts (4) Spotify 2019 summary graphic