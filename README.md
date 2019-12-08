# Sentiment_Anylysis_from_Scratch
Udacity's "Sentiment Anylysis from Scratch" implementation from the Nanodegree program NLP

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

The preprocessed reviews (train and test) are then stored to the cache (cache file: bow_features.pkl)

__Step 3: Extracting Bag-of-Words features__
Each document is transformed into a Bag-of-Words feature representation.

The dictionary or vocabulary  𝑉  (set of words shared by documents in the training set) used here will be the one on which we train our supervised learning algorithm. Any future test data must be transformed in the same way for us to be able to apply the learned model for prediction.

As the set of words in the training is not the same as the test set, unknown words ignored or replaced with the special <UNK> token.

__Step 4: Classification__
The data is trained on a Naive Bayes classifier from scikit-learn (GaussianNB)
