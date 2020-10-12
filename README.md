# Background

Twitter is widely used in sentiment analysis to help predict securities price movements and market behaviors.
Previous work has shown that behaviors in the financial markets are affected by President Trump's tweets.

The goal of this project is to determine whether there exists a similar behavior in short-term changes in the prices of financial securities immediately following Trump's tweets.

# Data
Sets from a period of less than one year were collected from the Trump Twitter Archive.
Set of COMEX Gold, NYMEX WTI Crude Oil, and ICE US Dollar Index futures contracts from Bloomberg terminal.

# Methods
Gensim Word2Vec Model: Based on Trump's tweets from inauguration day (01/20/2017) to 12/01/2019.
1. K-Nearest Neighbors
- Find minimum cosine distance between vectors of test data with training data and classify by nearest neighbors
2. Naive Bayes
- Word2vec vectors as features for target predictions with 0, 1, -1's.
3. Support Vector Maachine (SVM)
- Same methood implemented as with Naive Bayes.

# Libraries
numpy, scipy, pandas, re, math, nltk, gensim, sklearn, keras.
