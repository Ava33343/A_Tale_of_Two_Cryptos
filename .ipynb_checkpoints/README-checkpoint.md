# Unit 12— A Tales of Two Cryptos

![Stock Sentiment](Images/sentimental.jpeg)

## Background



Complete the following tasks:

1. [Sentiment Analysis](#Sentiment-Analysis)
2. [Natural Language Processing](#Natural-Language-Processing)
3. [Named Entity Recognition](#Named-Entity-Recognition)



### Instructions

#### Sentiment Analysis

Use the [newsapi](https://newsapi.org/) to pull the latest news articles for Bitcoin and Ethereum and create a DataFrame of sentiment scores for each coin.

Use descriptive statistics to answer the following questions:

> Which coin had the highest mean positive score?
>   * Bitcoin has the higher mean positive score compared to ethereum, 0.074 vs. 0.065.
>
> Which coin had the highest negative score?
>    * Based on the descriptive statistics, Ethereum has the highest compound score.
>        * It topped at 0.90 vs. the maximum compound score of 0.79 from Ethereum. 
>    * On the other hand, Bitcoin has compound scores higher than Ethereum on 
>        * its average, minimum, 25th, 50th and 75th percentiles.
>
> Which coin had the highest positive score?
>    * Ethereum has the highest positive score with its maximum at 0.21 rather than the 0.14 received by Bitcoin.
>   
> _*Sentiments towards Ethereum are more volatile as the standard deviations are higher than those for Bitcoin*_
> _*on scores for compound, negative, neutral and positive texts.*_

#### Natural Language Processing

In this section, you will use NLTK and Python to tokenize the text for each coin. Be sure to:

1. Lowercase each word
2. Remove punctuation
3. Remove stop words

Next, look at the ngrams and word frequency for each coin.

1. Use NLTK to produce the ngrams for N = 2.
2. List the top 10 words for each coin.

Finally, generate word clouds for each coin to summarize the news for each coin.

![btc-word-cloud.png](Images/btc-word-cloud.png)

![eth-word-cloud.png](Images/eth-word-cloud.png)



#### Named Entity Recognition

In this section, you will build a named entity recognition model for both coins and visualize the tags using SpaCy.

![btc-ner.png](Images/btc-ner.png)

![eth-ner.png](Images/eth-ner.png)

- - -

### Resources

[Vader Sentiment Analysis](http://www.nltk.org/howto/sentiment.html)

- - -


- - -

### Files

[Crypto Notebook](Answers/Code/crypto_sentiment.ipynb)

- - -

# References:
* CU Fintech Bootcamp GitLab Repository
* https://www.geeksforgeeks.org/python-lemmatization-with-nltk/
* https://riptutorial.com/nltk/example/27393/porter-stemmer
* https://newsapi.org/
* https://stackoverflow.com/questions/51102205/how-to-know-the-labels-assigned-by-astypecategory-cat-codes
* https://pandas.pydata.org/pandas-docs/stable/user_guide/categorical.html
* https://matplotlib.org/3.1.1/gallery/lines_bars_and_markers/bar_stacked.html#sphx-glr-gallery-lines-bars-and-markers-bar-stacked-py