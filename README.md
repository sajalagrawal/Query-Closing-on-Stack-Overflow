# Query-Closing-on-Stack-Overflow

## Problem Statement
Stack Overflow (SO) is a website specifically designed to help the users get answers to the programming
related questions posted by them. As the number of questions is increasing everyday, it is very important for the SO community to
maintain the quality of the questions in order to serve the users with quality content. And hence questions found to be of low
quality as per the community guidelines are closed. The process of closing questions is not completely automated and hence it is a
tedious task for the moderators. This work proposes a classifier to automate the process of closing questions on SO and to let
the user know that the posted question has high probability to get closed. 

We have developed machine learning classifiers for predicting whether a user query on SO will be closed or not and if closed, its reason for closure.


## Datasets
We used StackExchange Data Explorer to pull out closed questions with their user data from publicly available Stack Overflow dump. We also used Google BigQuery which is a RESTful web service for analysing and downloading huge datasets.

## Solution
On the basis of analysis of the dataset, we have employed the following classification algorithms for predicting whether a question is likely to be closed or not-
* Logistic Regression
* Random Forest
* Support Vector Machine

For the second classification task for predicting the reason for closure, we have employed the following classification models-
* Logistic Regression
* Random Forest
* Support Vector Machine
* AdaBoost

## Results
For the first classification task - SVM with RBF Kernel outperforms the rest with an accuracy and F1-score of 91.32% and 0.91 respectively.

For the second classification task - Our AdaBoost model could achieve an accuracy of 43.19% and F1-score of 0.42.
