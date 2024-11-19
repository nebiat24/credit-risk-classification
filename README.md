# credit-risk-classification
This repository is for the Data Analytics Bootcamp Module 20 Challenge
# Overview of the Analysis
For this assignment, I used various techniques to train and evaluate a supervised machine learning model based on loan risk. I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* The purpose of this analysis is to create a model that can correctly gauge whether or not a person will be a healthy or high-risk loan candidate.
* I used a dataset from a peer-to-peer lending services company to create this model.
* This dataset contains several factors that may affect the health of a loan, such as income, debt, and debt to income ratio.
* Using this dataset, I was able to split the data into training and testing categories, then run the training set through the logistic regression model.
* Once the model made its predictions, I was able to confirm the results by determining the balanced accuracy score, viewing the confusion matrix, and creating a classification report.
* I also oversampled the data and ran predictions again, confirming the results on a larger dataset.


## Results

* Machine Learning Model 1-using the original dataset:
  * Balanced accuracy score: 94%
  * Precision: 100% healthy loans, 87% high-risk loans
  * Recall: 100% healthy loans, 89% high-risk loans
![original](Credit_Risk/Images/original_data.PNG)


* Machine Learning Model 2-using the oversampled dataset:
  * Balanced accuracy score: 99%
  * Precision: 100% healthy loans, 87% high-risk loans
  * Recall: 100% healthy loans, 100% high-risk loans
![oversampled](Credit_Risk/Images/oversampled_data.PNG)

## Summary

I believe that this model would be appropriate to determine loan risk, if left open to human interpretation/review.
* The model yields high accuracy scores when run on both the original and oversampled datasets.
* While the accuracy, precision, and recall are all higher when the model determines a healthy loan candidate, the model is still fairly accurate at determining a high-risk candidate. As long as borderline candidates can be left open to additional research and interpretation, I believe this would be a useful tool when deciding loan risk.
