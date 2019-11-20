# The *Instant Gratification - Predict the Class* Challenge on www.kaggle.com

##  Introduction
I chose this challenge because I wanted a problem with moderately large dataset. This challenge has 200,000+ training examples and requires predicting target class for 100,000+ test examples. I had to *learn* to use the relevant libraries that help manipulate large sized datasets with limited computing resources. However, as I got further in my attempt, I realized that this was a problem that tested more the ability to perform and learn from exploratory data analysis rather than managing large sized dataset. 

In this project, I have focussed on applying multiple machine learning algorithms to the given dataset with a goal of reviewing their relative efficacy for binary classification of the test dataset. I have applied 3 different algorithms - Penalized Logistic Regression, Naive Bayes Regression and Quadratic Discriminant Analysis.

The project is implemented in R.

##  The Challenge
The reasons that this makes an excellent case study especially for new practitioners on machine learning:
1.  **Dealing With Large Sized dataset** - This a good challenge if the goal is to learn how to manage a large dataset using limited computing resources. In my solution, I have used the `ff` and `ffbase` libraries that provide excellent functionality to manage large datasets.
2.  **Importance of EDA* - This challenge comes with a twist and requires careful exploratory data analysis and consequent hypotheses formulation. The key to the whole challenge is in realizing one distinctive characteristic of the dataset and the rest of the solution is almost trivial.

##  My approach
The focus of my approach is to understand the relative efficacy of the different learning algorithms. Equally importantly, I was not focussed on *winning* the challenge but on using this as an opportunity to learn how a challenge may be addressed in a real-life situation.

The first part of my solution focusses on data wrangling 
1.  Performing exploratory data analysis (EDA) on the train data-set to get better sense of the data and form preliminary hypotheses.
2.  I had to perform multiple EDA passes as some of the early hypthesis didn't prove useful.

The second part of my solution applies three learning alogrithms, Penalized Logistic Regression, Naive Bayes Regression and Quadratic Discriminant Analysis to build learning models. The goal was to estimate the prediction accuracy of these three algorithms and also pick the best of the lot. 

For each of the learning algorithm I estimated the test set prediction AUC and in the final (third) part I used the top performing algorithm - Quadratic Discriminant Analysis -  to make predictions for the *test* dataset. I used Kaggle's evaluation engine to get final verified results of the performance of the chosen algorithm.

##  The Directory Structure
The entire project is available either as a single .Rmd document `Instant-Gratification.Rmd` in the root directory or split into 3 sections, paralleling the discussion above, in the `/scripts` directory. The data, given its relatively large size, is not included in this repo but can be easily got from https://www.kaggle.com/c/instant-gratification. Finally the `/RDA` directory contains the RData created and used by the code in the 3-sections version. Again this is not made available with this repo because of its relatively large size. However, anyone looking to replicate my approach with *create* the necessary RData files as part of the implementation.


