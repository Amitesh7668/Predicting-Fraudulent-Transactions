# Business Context
This case requires trainees to develop a model for predicting fraudulent transactions for a 
financial company and use insights from the model to develop an actionable plan. Data for the 
case is available in CSV format having 6362620 rows and 10 columns.
Candidates can use whatever method they wish to develop their machine learning model. 
Following usual model development procedures, the model would be estimated on the 
calibration data and tested on the validation data. This case requires both statistical analysis and 
creativity/judgment. We recommend you spend time on both fine-tuning and interpreting the 
results of your machine learning model.

# Candidate Expectations
### Your task is to execute the process for proactive detection of fraud while answering following questions.
1. Data cleaning including missing values, outliers and multi-collinearity. 
2. Describe your fraud detection model in elaboration. 
3. How did you select variables to be included in the model?
4. Demonstrate the performance of the model by using best set of tools. 
5. What are the key factors that predict fraudulent customer? 
6. Do these factors make sense? If yes, How? If not, How not? 
7. What kind of prevention should be adopted while company update its infrastructure?
8. Assuming these actions have been implemented, how would you determine if they work?

9. # Answers to the Questions

## Data cleaning including missing values, outliers and multi-collinearity.
 Since there were no missing values in the dataset, I did not need to perform any data cleaning related to that. I checked for multicollinearity using correlation analysis.If I remove outliers than it is removing our fraudulent main data for which we have to apply prediction.
 
## Describe your fraud detection model in elaboration.
Logistic Regression model working better with 99% accuracy, Since it's highly imbalanced and huge data it was hard to train tree models

This fraud detection model is based on Logistic Regression and Naive Bayes as it's a large dataset with a imbalance data.  logistic regression is an ensemble learning method that combines multiple logistic regression to make a final prediction.Each  logistic regression is trained on a different subset of the data and a different set of features. When making a prediction, the final prediction is made by averaging the predictions of all the  Logistic Regression.

## How did you select variables to be included in the model?
I selected variables to be included in the model based on domain knowledge and feature importance analysis.

## What are the key factors that predict fraudulent customer?
 The key factors we identified are that type_PAYMENT, type_CASH_IN, type_CASH_OUT , amount and newbalanceOrig are playing major   role to know is transaction is Fraud or not
 
 The fraud amount happen in very less time within 2 step

## Demonstrate the performance of the model by using best set of tools.
I evaluated the performance of the model using several metrics such as accuracy, precision, recall, F1 score. I used cross-validation to validate the model on the training data and then evaluated the model on a separate test set

## Do these factors make sense? If yes, How? If not, How not?
The factors i took definitly makes sense because i took care of preprocessing step such as null values, duplicates, multicollinearity, encoding, scaling etc.

## What kind of prevention should be adopted while company update its infrastructure?
To prevent fraud, companies can adopt several prevention measures such as implementing multifactorial authentication, monitoring transactions in real-time, and implementing machine learning models to detect and flag suspicious transactions. It is also important to regularly update security protocols and educate employees and customers about fraud prevention best practices.

## Assuming these actions have been implemented, how would you determine if they work?
This implementation will save time ,prevent to consume more storage in future if these kind of column will come they can lead to multicollinearity, overfit which may affect the accuracy
