# Report of Loan Analysis Model based on IA 

## Overview 


* Purpose of the analysis

This report describes various techniques used to train and evaluate a model based on loan 1risk to help a personal credit institution, to obtain the lending risk of each customer, based on historical data. 

* Data used 

  We will use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. 
  The next image describes the data considering 77,536 rows. 

<p align="center"><img src="https://github.com/zuntaalejandra/credit-risk-classification/blob/main/Credit_Risk/images/input_data.png" /></p>



## Stages of the machine learning process

* The main stages of the machine learning process used in this case are:

1) Create the labels set (`y`)  from the “loan_status” column of dataset, and   the features (`X`)  from the remaining columns:
* loan_size	
* interest_rate	
* borrower_income	
* debt_to_income	
* num_of_accounts	
* derogatory_marks	
* total_debt

2) Split the data into training and testing datasets 

3) Create a logistic regression model by using the training data

4) Save the predictions on the testing data labels 

5) Evaluate the model’s performance using this tools:

* The Accuracy score of the model
* A confusion matrix
* A classification report

After that, we will resample the dataset, to train another model and evaluate the result with the same tools. 

## Results of the Analysis


* Machine Learning Model 1 --> Accuracy, Precision, and Recall scores.

The next image describes the prediction values obtained in this model.

<p align="center"><img src="https://github.com/zuntaalejandra/credit-risk-classification/blob/main/Credit_Risk/images/Target_values_1.png" /></p>

The next image includes results for model 1.

<p align="center"><img src="https://github.com/zuntaalejandra/credit-risk-classification/blob/main/Credit_Risk/images/Confusion_Matrix_1.png"/><p>



* Machine Learning Model 2  --> Accuracy, Precision, and Recall scores.

The next image describes the prediction values obtained for model 2.

<p align="center"><img src="https://github.com/zuntaalejandra/credit-risk-classification/blob/main/Credit_Risk/images/Target_values_2.png" /></p>

The next image describes the prediction values obtained in model 2.

<p align="center"><img src="https://github.com/zuntaalejandra/credit-risk-classification/blob/main/Credit_Risk/images/Confusion_Matrix_2.png"/><p>


## Summary

* Which one seems to perform best? How do you know it performs best?

For model 1, Based on the recall score obtained of 91% for 1 value and 99% of 0 value, we can say, that is a reliable model.

Based on Classification Report form model 2, the recall result for 1 values is 0, so it is not a good model. By the other hand, Confusion Matrix is printed with 0, for predicted 1 value. The conclusion is that is not a good model.


* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

A good model must work with great accuracy, predicting 0 an 1 values as well.  Is is very important.