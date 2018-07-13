# Scipy Day 3 Notes #

## Keynote - The Role of Python in Recent Grav Wave Astronomy ##

## Recipe2Vec ##

* GloVe word word co-occurence matrix
* Word2vec from Google (skip-gram and continous bow)
* this one uses word2vec
* t-SNE - won a Kaggle award :)
* http://tasty.co

## scikit-learn and tabular data ##

* Mind the Gap talk from Augsburger
* scikit-learn transformers + models = pipelines
* Pandas df doesn't work well with piplines due to objects
* There are encoding work arounds
* one-hot/dummy encoding - codes are broken out to columns represented by boolean
* scikit-learn now has the encoders in preprocessing
* ColumnTransformer - apply transformer onto specific columns
* sklearn-pandas package
* ibex - pandas adaptors for scikit-learn -- transform estimators to pandas-aware estimators
