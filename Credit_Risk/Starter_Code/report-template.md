# Module 20 Report Template

## Overview of the Analysis

This project will take a look at lending companies. In order for their business to become successful they will need to know that they will be able to either return the asset or get the repayment back. Credit risk analysis is a good way for companies to make a more informed decision in these types of matters.

Using a machine learning model, I will try to determine which loans are healthy loan `0` and  high-risk loan `1` based on the loan status provided by the lending company, as well as if there are any false healthy loans (false positives) as well as false high-risk loan (false negatives).

First we will split the data into training and testing sets. Then we will create a logistic regression model with the original data. We will use the function of LogisticRegression (creating the logistic regression model), confusion_matrix (Compute confusion matrix to evaluate the accuracy of a classification.), and train_test_split (Split arrays or matrices into random train and test subsets.) and display the data with classification_report (Build a text report showing the main classification metrics).



## Results

Results from the Machine Learning Model:

![image](https://github.com/Mikelmillz/credit-risk-classification/assets/145722846/1bf307ec-6219-4e61-86bb-d55824a7ce52)


We can see that The Logistic Regression model predicted healthy loans 100% of the time and predicted non-healthy loans 84% of the time.

According this models recall scores, the model made 1% of mistakes when predicting healthy loans and made 9% of mistakes when predicted non-healthy loans.


## Summary

Model fitted from the original data:

![image](https://github.com/Mikelmillz/credit-risk-classification/assets/145722846/9137bd71-0edf-4fa5-b50f-bbc520243f32)

563 correctly classified high-risk loans. 56 false negative, meaning the actual value is healthy and the predicted value is non-healthy. 

18663 correctly classified healthy loans. 102 false positive meaning the actual value is non-healthy and the predicted value is healthy.

If this were me, I would be fine with using this model. This is because I would rather a loan be marked as high risk and actually be a  healthy loan as there would shouldn't be much monetary loss since they should have been marked as a healthy loan to begin with. Since the healthy loans got a 99% accuracy, even though there were more of these than false high-risk loans, the accuracy is very high. 

With all of this I would still want to try and find another model that had a higher percentage than 91% for the recall score on the high-risk loans.
