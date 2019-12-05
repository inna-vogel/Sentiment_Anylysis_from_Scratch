# Sentiment_Anylysis_from_Scratch
Udacity's "Sentiment Anylysis from Scratch" implementation from the Nanodegree NLP

__Step 1: Data__
The dataset used is the IMDb dataset. It consists of movie reviews from the website imdb.com, each labeled as either 'positive', if the reviewer enjoyed the film, or 'negative' otherwise.

Maas, Andrew L., et al. Learning Word Vectors for Sentiment Analysis. In Proceedings of the 49th Annual Meeting of the Association for Computational Linguistics: Human Language Technologies. Association for Computational Linguistics, 2011.

__Step 2: Preprocessing__
a) Remove HTML tags
b) Remove non-letter characters
c) Normalize uppercase letters by converting them to lowercase
d) Tokenization
e) Removing stop words
f) Stemming words in each document.

__Step 3: Extracting Bag-of-Words features__
Each document is transformed into a Bag-of-Words feature representation

As the set of words in the training is not the same as the test set, unknown words ignored or replaced with the special <UNK> token.
