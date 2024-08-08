# Capstone-Project-Sentiment-Analysis
# -- Sentiment Analysis on Musical Instrument --

# introduction

A sentiment is an attitude, belief, or conclusion brought on by a sensation. Sentiment analysis, commonly referred to as opinion mining,
examines how individuals feel about particular things. Through different social media, including forums, microblogs, and online social
networking sites, users may publish their own material. Many social media platforms disclose their application programming interfaces
(APIs), which motivates academics and developers to gather and analyse data. However, there are a number of issues with those online
data sources that can make sentiment analysis more difficult. The quality of people's opinions cannot be ensured because they are
allowed to upload their own information, which is the first issue. The second problem is that such internet data's actual source is not
always known. A ground truth is more akin to a label placed on an opinion, designating whether it is favourable, unfavourable, or
neutral.

# Data Overview

Amazon.com reviews on products were gathered between May 1996 and July 2014. Each review consists of the following information:
1) Reviewers ID, 2) Product Code, 3) Score, 4) Review Period, S) Review Supportiveness, and 6) Review Text. There are no half-stars
or quarter-stars because all ratings are based on a 5-star system, and all ratings.

# Implementation

1. Data Preprocessing-

As the first step for any data mining method, dataset was evaluated and preprocessing techniques were applied to prepare
the data for mining. The Dataset contained 10,262 records.These records were analyzed for their distribution of unique
values for products and customers. The dataset was also analyzed for columns having blank values.

The dataset was also analyzed for distribution of ratings.Histograms for each value of rating from the column ‘overall’

WordCloud was implemented as part of analysis of the reviews to get an idea about the words most frequently found in the best
and worst ratings.

2. Preparing Train and Test Sets-
   
After selecting samples from each class, the dataset was split into Train and Test data with a split ratio of 0.8, i.e., 80 percent
of the data was used for training and 20 percent for testing. The data was shuffled while doing the split so that any possible bias
could be eliminated from the order in which the training data would be loaded.
 
4. Training the Model-
   
To use the Logistic Regression - The built-in en_core_web_sm NLP pipeline has been used in the implementation.

6. Evaluating the Model-
   
The performance of the model was evaluated after each iteration of the training. The model was evaluated with test data,
which was created during the dataset split. To shows a snapshot of iterations of training and model evaluation listing
the Loss, Precision, Recall and F-Score.

7. Accuracy Report Values
   
After the model training, the final scores for the accuracy 'for different-different Algorithm' report of the model are listed as below:

ACCURACY REPORT FOR THE MODEL

Logistic Regression Test Accuracy: 0.8810059200798708

Decision Tree Test Accuracy: 0.8127867271771336

KNN Test Accuracy: 0.8791539733245264

SVC Test Accuracy: 0.8795439317757772

Naive Bayes Test Accuracy: 0.8038184420263036


