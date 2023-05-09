# Credit-Risk-Classification

**Overview of the Analysis**

The purpose of this activity  is to compare 2 machine learning models based on its ability to detect loan risks. The data included each individual's income, loan and debt amount, number of accounts, interest rate, and number of deragatory marks. Their loan status is what we need to predict if said person will be a loan risk. 

Loan status was used for estimation and prediction (y) and the remaining data was used as the features set (X). A count of the y values was used to see out many indivduals were actually loan risks or not. 

Each X and y variables were split into testing and training data. The training data was used to create a Logistic Regression model. Once the model was fit using the training data, predictions were made using the test data (X) to determine how accurate the fitted model was at predicting loan risks. 

Resampling was also used as a machine learning model. This ensured that the 'y' labels have an equal number of data points. The resampled training data was used with the Logistic Regression model to also make predictions


**Results**


* Machine Learning Model 1 - Logistic Regression with original data:
  * Accuracy: 0.99 (99%) - The model's predicted outcomes were 99% correct compared to the total number of outcomes.
  * Precision: 0.85 (85%) - For all the individuals who were classified by the model as being a loan risk, 85% were actually a loan risk.
  * Recall: 0.91 (91%) - Of all of the actual people who are loan risks, this model correctly classified individuals as loan risks 91% of the time.


* Machine Learning Model 2 - Logistic Regression with resampled training data (RandomOverSampler):
  * Accuracy: 0.99 (99%) - The model's predicted outcomes were 99% correct compared to the total number of outcomes
  * Precision: 0.99 (99%) - For all the individuals who were classified by the model as being a loan risk, 99% were actually a loan risk
  * Recall: 0.99 (99%) - Of all of the actual people who are loan risks, this model correctly classified individuals as loan risks 99% of the time

**Summary**

The Logisitic Model using the resampled data works the best predicting who will be a potential loan risk. Though both models were 99% accurate overall, the resampled data was more precise (+14%) at predicting loan risks compared to those who were actually loan risks. It also was yeilded a higher recall score by 9%. 
I would recommend using the Logistic Regression model with resampled data for this problem. It is no better to reject a loan from an individual who is not a loan risk, than it is to give a loan to an individual who is not in good standing; either way, the comapny will lose out on money. The model with the highest accuracy, most precise, and highest recall score is the best fit. 
