# Module 20 Challenge : Supervised Learning

# Background

The objective of this project is to train and evaluate a model that can accurately assess loan risk using various techniques. The dataset used for analysis comprises of previous lending activities from a peer-to-peer lending services company. The goal is to create a model that can determine the creditworthiness of borrowers with precision. 

Upon importing a CSV file, the data should be separated into labels and features. The `loan_status` column should be used as the label (y), while the remaining columns should be used as features (X). A value of 0 in the `loan_status` column indicates that the loan is healthy, while a value of 1 indicates that the loan has a high risk of defaulting. The next step is to split the data into training and testing using the `train_test_split` function.

In order to create a regression model, it is recommended to employ the logistic regression model when dealing with binary data. The process of fitting the regression model involves assigning the model and subsequently utilizing the training data. Once the model has been trained, predictions can be made using the testing data. Finally, it is necessary to create a confusion matrix and classification report. To accomplish this, it is essential to import the relevant dependencies, namely `confusion_matrix` and `classification_report` respectively. 


# Results

* **Confusion matrix**

![image](https://github.com/lakigit/credit-risk-classification/assets/138610916/1babec63-7f6b-4c9b-883f-24c6e2bedba4)

According to this confusion matrix, 

* True Negative (TN): 18663 instances were correctly classified as "Healthy Loan."
* False Positive (FP): 102 instances were incorrectly classified as "High-Risk Loan" when they were actually "Healthy Loan."
* False Negative (FN): 56 instances were incorrectly classified as "Healthy Loan" when they were actually "High-Risk Loan."
* True Positive (TP): 563 instances were correctly classified as "High-Risk Loan."


* **Classification Report**

![image](https://github.com/lakigit/credit-risk-classification/assets/138610916/5cfc167b-b1d7-438d-b30a-c4c0673112fe)

1. Precision:
For "Healthy Loan": 100% (or 1.00)
For "High-Risk Loan": 85% (or 0.85)

2. Recall (Sensitivity):
For "Healthy Loan": 99% (or 0.99)
For "High-Risk Loan": 91% (or 0.91)

3. F1-score:
For "Healthy Loan": 100% (or 1.00)
For "High-Risk Loan": 88% (or 0.88)

4. Support:
The number of instances in each class: 18765 for "Healthy Loan" and 619 for "High-Risk Loan."

5. Accuracy:
Overall accuracy of the model: 99% (or 0.99)

6. Macro Avg:
The average of precision, recall, and F1-score across both classes.

7. Weighted Avg:
The weighted average of precision, recall, and F1-score, considering the number of instances in each class.

`Conclusion` : 

* The model seems to perform exceptionally well, especially for the "Healthy Loan" class, with high precision, recall, and F1-score.
* For the "High-Risk Loan" class, the model is slightly less accurate, with lower precision, recall, and F1-score compared to the "Healthy Loan" class.
* The overall accuracy of 99% suggests that the model is effective in predicting both classes.