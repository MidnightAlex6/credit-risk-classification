# credit-risk-classification

## Background

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Overview of the Analysis

The purpose of this analysis is to build a machine learning model using logistic regression to predict loan status for the company. The dataset contains various features related to borrowers' financial information, such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. By training the model on historical data with known loan statuses, the company aims to use it for future loan applications to automate the decision-making process and identify potential defaulters.

#### Results

* Accuracy Score: The accuracy score of the machine learning model on the training data is approximately 0.99, which means it correctly predicted 99% of the loan statuses in the training set.

* Precision Score: For class 1 (high-risk loan), the precision score is approximately 0.86. It means that out of all the predicted defaults, around 86% were actually true defaults, and the remaining 14% were false positives. For class 0 (healthy loan), the precision score is approximately 1.00. It means that out of all the predicted healthy loans, 100% were actually true healthy loans. 

* Recall Score: The recall score for class 1 is approximately 0.90, indicating that the model correctly identified around 90% of the actual loan defaults out of all the true positives and false negatives. The recall score for class 0 (healthy loan) is 1.00, indicating that the model correctly identified 100% of the actual healthy loans out of all the true positives and false negatives. 

#### Summary

The machine learning model based on logistic regression has shown excellent performance on the training data, achieving high accuracy, precision, and recall scores. It accurately predicted the majority of loan statuses and successfully identified a significant portion of the actual defaults. These results are promising and demonstrate the model's capability to distinguish between high-risk loans and healthy loans.

#### Recommendation

Considering the high accuracy and reasonable precision and recall scores on the training data, the logistic regression model appears to be a viable choice for predicting loan statuses. Its performance suggests that it can effectively assist the company in making loan approval decisions, identifying potential risks, and reducing manual processing time. However, it is crucial to evaluate the model's performance on the testing data to ensure its generalisation to new, unseen data. If the model performs well on both training and testing data, it can be confidently recommended for use by the company to enhance their loan application process. Regular monitoring and updating of the model as new data becomes available will be essential to maintain its predictive accuracy over time.


## Instructions

The instructions for this Challenge are divided into the following subsections:

* Split the Data into Training and Testing Sets

* Create a Logistic Regression Model with the Original Data

* Write a Credit Risk Analysis Report

### Split the Data into Training and Testing Sets

Open the starter code notebook and use it to complete the following steps:

1. Read the `lending_data.csv` data from the Resources folder into a Pandas DataFrame.

2. Create the labels set (`y`) from the “loan_status” column, and then create the features (`X`) DataFrame from the remaining columns.

    > **Note:** A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

3. Split the data into training and testing datasets by using `train_test_split`.

### Create a Logistic Regression Model with the Original Data

Use your knowledge of logistic regression to complete the following steps:

1. Fit a logistic regression model by using the training data (`X_train` and `y_train`).

2. Save the predictions for the testing data labels by using the testing feature data (`X_test`) and the fitted model.

3. Evaluate the model’s performance by doing the following:

    * Generate a confusion matrix.

    * Print the classification report.

4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

### Write a Credit Risk Analysis Report

Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the `README.md` file included in your GitHub repository.
