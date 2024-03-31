# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The aim of this analysis is to employ diverse methodologies for training and assessing models dealing with imbalanced class distributions. Utilizing a dataset comprising past lending transactions from a peer-to-peer lending firm, the objective is to construct a model capable of discerning the creditworthiness of borrowers.
* Our financial data was from the lending data CSV file which includes features: loan size, interest rate, borrower income, debt to income ratio, # of accounts, derogatory marks, and total debt. Using these features, predictions were made to classify loans as healthy or high risk.
* In this analysis, the varaible being predicted was 'loan_status', which we also implemented the 'value_counts' function to get a reutn of series containing counts of unique values. 
* The stages of this analysis include:
  * Splitting the data in Training and Testing Sets
  * Creating Logistic Regression Model with Original Data
  * Predict a Logistic Regression Model with Resampled Training Data
* In this analysis we used the Logisitic Regression method. Logistic regression is a statistical method used for binary classification tasks, where the outcome variable is categorical and has only two possible outcomes (e.g., yes/no, true/false, 1/0). It models the probability that an observation belongs to a certain category based on one or more predictor variables. In this scenario, this method was used to classify loan statuses.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1: Logistic Regression Model with Original Data
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    * Accuracy: 95.2%
    * Precisions: 100% for Healthy Loans(0) and 85% for High-Risk Loans(1)
    * Recall Score: 99%



* Machine Learning Model 2: Logistic Regression model with Resampled Training Data
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    * Accuracy: 99.3%
    * Precisions: 100% for Healthy Loans(0) and 84% for High-Risk Loans(1)
    * Recall Score: 99%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
  * Both Models performed well, however I would say that Model 2 with the resample training data had better performance due to its higher accuracy score and f-1 scores. For these reaons, I would choose recomment Model 2.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
  * The main problem we are trying to solve is targeted at correctly predicting the High-Risk Loans(1). With that being said, performance is definitely dependent on that, and both models performed similarly with Model 1 having a higher precision score by 1%.

If you do not recommend any of the models, please justify your reasoning.
