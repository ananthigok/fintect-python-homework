# Unit 12—Tales from the Crypto

![Stock Sentiment](Images/sentimental.jpeg)

## Background

There's been a lot of hype in the news lately about cryptocurrency, so you want to take stock, so to speak, of the latest news headlines regarding Bitcoin and Ethereum to get a better feel for the current public sentiment around each coin.

In this assignment, natural language processing was applied to understand the sentiment in the latest news articles featuring Bitcoin and Ethereum. Also applied fundamental NLP techniques to better understand the other factors involved with the coin prices such as common words and phrases and organizations and entities mentioned in the articles.

The following tasks are done:

1. [Sentiment Analysis](#1---Sentiment-Analysis)
2. [Natural Language Processing](#2---Natural-Language-Processing)
3. [Named Entity Recognition](#3---Named-Entity-Recognition)

---

## Files

[Starter Notebook](Starter_Code/crypto_sentiment.ipynb)

---

## Instructions

### 1 - Sentiment Analysis

Using the [newsapi](https://newsapi.org/) to pull the latest news articles for Bitcoin and Ethereum and created a DataFrame of sentiment scores for each coin.

The following questions were answered using descriptive satistics:

> Which coin had the highest mean positive score?
>
> Which coin had the highest negative score?
>
> Which coin had the highest positive score?



### 2 - Natural Language Processing

In this section, NLTK and Python was used to tokenize text, find n-gram counts, and create word clouds for both coins. 

#### Tokenized with the below points

1. Lowercased each word.
2. Removed punctuation.
3. Removed stop words.

#### N-grams

Next, looked at the ngrams and word frequency for each coin.

1. Used NLTK to produce the ngrams for N = 2.
2. Listed the top 10 words for each coin.

#### Word Clouds

Finally, generated word clouds for each coin to summarize the news for each coin.

![btc-word-cloud.png](Images/btc-word-cloud.png)

![eth-word-cloud.png](Images/eth-word-cloud.png)


### 3 - Named Entity Recognition

In this section, a named entity recognition model was built for both coins and visualized the tags using SpaCy.

![btc-ner.png](Images/btc-ner.png)

![eth-ner.png](Images/eth-ner.png)



### Resources

[Vader Sentiment Analysis](http://www.nltk.org/howto/sentiment.html)