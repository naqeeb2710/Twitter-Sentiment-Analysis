# Twitter Sentiment Analysis
This is a Python notebook for performing sentiment analysis on Twitter data. The notebook uses two methods to extract tweets from Twitter: one using Selenium library and the other using snscrape library. It also uses the textblob library to perform sentiment analysis on the extracted tweets.

## Selenium Method
The first method uses Selenium to authenticate and connect to the Twitter website. It then uses Selenium to search for tweets containing a given keyword or hashtag and scrolls down the page to load more tweets. Once the tweets are extracted, the textblob library is used to perform sentiment analysis on the tweets.

## Snscrape Method
The second method uses the snscrape library to extract tweets directly from the Twitter API without the need for authentication. It also allows for searching for tweets containing a given keyword or hashtag. Once the tweets are extracted, the textblob library is used to perform sentiment analysis on the tweets.

## Preprocessing and Sentiment Analysis
Before performing sentiment analysis, the notebook first preprocesses the tweets by removing URLs, special characters, and other unwanted text. The textblob library is then used to perform sentiment analysis on the cleaned tweets, and a polarity score is assigned to each tweet.

The sentiment analysis assigns a polarity score to each tweet, indicating whether the tweet is positive, negative, or neutral. The scores range from -1 to 1, with -1 being very negative, 1 being very positive, and 0 being neutral. The notebook also displays a histogram of the polarity scores to give an overview of the sentiment of the extracted tweets.

## Hashtag Analysis
The notebook then extracts the most frequently occurring positive and negative hashtags from the extracted tweets. This gives an idea of the topics that people are tweeting about in a positive or negative manner.

## Classification Model
Finally, the notebook uses the scikit-learn library to train a classification model on the extracted tweets. The model is trained on a labeled dataset of tweets, where each tweet is labeled as either positive, negative, or neutral. The model achieves an accuracy of 82% on a test set of tweets, which is a decent performance for a sentiment analysis model.

## Prerequisites
Before running the notebook, you will need to install the following libraries:

``` 
Selenium: 
snscrape:
textblob: 
scikit-learn: 
pandas:
matplotlib:
wordcloud
nltk
```

## Running the Notebook
To run the notebook, simply open the main.ipynb file in a Jupyter Notebook environment and run each cell in order. Make sure to enter your Twitter API credentials in the appropriate cell to authenticate and connect to the Twitter API (only for snscrape method).