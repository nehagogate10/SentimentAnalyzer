# Sentiment Classification
### By: Neha Gogate

# Description
A binary sentiment analyzer that automatically classifies input text as portraying either positive or negative sentiment.

### baseline_BoW.ipynb
As my baseline system, I utilized the bag of words (BoW) model. My preprocessing techniques consisted of removing punctuation and making the text data lowercase. I utilized CountVectorizer, and then calculated this model's f1, precision, recall, and accuracy with the Gaussian Naive Bayes classifier. 

### improved_unigrams.ipynb
This is an improved version of my baseline bag of words model. It is similar to the baseline model conceptually, with the addition of several more preprocessing steps in order to remove aspects that did not add value to the machine learning models. This included removing all stop words,  words with a length of less than or equal to 2,  all numbers, and  all words that only consist of underscores, an issue specific to this corpus. I used CountVectorizer, and then calculated this model's f1, precision, recall, and accuracy with the Gaussian Naive Bayes, Decision Tree, Stochastic Gradient Descent, Logistic Regression, and Perceptron classifiers.

### improved_bigrams.ipynb
These preprocessing techniques were consistent with those in previous models, and included removing all stop words, words with a length of less than or equal to 2, all numbers, and all words that only consist of underscores. Then I implemented CountVectorizer with bigrams. Again, its f1, precision, recall, and accuracy were calculated with the Gaussian Naive Bayes, Decision Tree, Stochastic Gradient Descent, Logistic Regression, and Perceptron classifiers.

### improved_trigrams.ipynb
I used similar preprocessing techniques as the improved bigram model. CountVectorizer is implemented with trigrams, and the f1, precision, recall, and accuracy values were calculated with the Gaussian Naive Bayes, Stochastic Gradient Descent, and Perceptron classifiers, as these three performed best.

### improved_POStagger.ipynb
Here, I implemented similar preprocessing techniques to the other four models. I then used the pos_tag functionality from nltk to get the pos tags of each word in the text data, and used that information for sentiment analysis. The logic behind this method is that the frequent occurrences of certain pairs of part-of-speech tags would provide insight into whether positive and negative sentiments could be detected from sentence structures. I used CountVectorizer to create the POS tag bigrams, and then calculated the f1, precision, recall, and accuracy with the Gaussian Naive Bayes, Decision Tree, Stochastic Gradient Descent, Logistic Regression, and Perceptron classifiers.

# Running Code
In order to run each of these five jupyter notebooks  (baseline_BoW.ipynb , improved_unigrams.ipynb, improved_bigrams.ipynb, improved_trigrams.ipynb, improved_POStagging.ipynb), simply simply click Kernel -> Restart and Run All (located in the top bar).
