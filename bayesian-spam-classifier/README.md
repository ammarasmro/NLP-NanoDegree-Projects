# Bayesian Spam Classifier for SMS 

This mini project shows the use of different methods to train classifiers that can detect spammy sms messages. The same model can be used to detect spammy emails too.

Spam detection is a supervised learning problem as we try to train models that map input text into output labels (spam or not-spam). The data is obtained from the UCI machine learning repository. 

## Data Preprocessing

The steps taken to preprocess our data and make it ready for a sklearn classifier consisted of turning categorical labels into numbers, 0 and 1

Text | Numerical
--- | ---
Spam | 1
Not-Spam | 0

## Data Representation

To feed the textual data into sklearn models we need to find a represtation that uses numbers. For this project we use *Bag-of-Words (BoW)*. 

Each sms is simply feed into a counter to make a frequency distribution matrix so the documents will be represented by vectors of integer word counts. Sklearn provides the count vectorizer functionality to ease this task.

## Training

The algorithm used for classification is the Naive Bayes. It is chosen for its simplicity and the fact that it treats each word as an independent feature.

## Evaluation

The resulted evaluations show that even with a simple technique we can obtain really good results without having to use more complex and computationally expensive models

Metric | Score
--- | ---
Accuracy | 0.9885139985642498
Precision | 0.9720670391061452
Recall | 0.9405405405405406
F1 | 0.9560439560439562

## Next Steps

-[ ] Train an RNN model that uses Embeddings to see if using a more complex model is worth the effort.
-[ ] Try an email dataset to see how this method performs for longer text



