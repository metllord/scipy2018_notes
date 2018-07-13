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

## Safe Handling Instructions for Missing Data ##

* https://wirepedia.org
* https://github.com/deniederhut/safe-handling-instructions-for-missing-data
* missing data introduces bias into the data
* missing data level of bias from less to most: missing completely at random - missing at random - missing not at random
* big data excentuates the missing data problem
* you can't/shouldn't always drop missing rows
* missing data in one observation throws off other features
* don't use the mean.

0. Stop collecting missing data - easier to get the missing data then fix it later.
    - track the province of the data; keep all forms of it
1. collect auxiliary features- variables not planned on using but have strong correlation with the wanted feature
    - ex: get zipcode and education level in addition to income
2. establish your regime
3. Use modern MI technique - multiple imputation (missforest, MO, MICE)
    - do this 5 to 10 times
4. run your analysis
5. report all the things
    - include missing value info; number, descriptive stats, techiques

