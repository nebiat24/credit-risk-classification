# Credit Risk Analysis Report
## Overview of the Analysis
The goal of this analysis is to assess the credit risk of loan applicants using a machine learning model. The dataset used for this analysis includes features about loan applicants and their credit history, with the objective of predicting whether an applicant is a high-risk (Class 1) or low-risk (Class 0) borrower. The purpose of this analysis is to build a reliable model that can accurately predict the credit risk of loan applicants, assisting financial institutions in making informed lending decisions.

### Steps Taken:

1.   Data preprocessing and feature engineering to prepare the dataset.

2.   Split the data into training and testing sets.

3.  Applied a logistic regression model to classify the loan applicants.

4.  Oversampled the minority class to address the class imbalance.

5.  Evaluated the model's performance based on various metrics.


# Results

- **Accuracy Score:** 1.00
The model correctly predicted the loan class for all data points, achieving 100% accuracy. However, this high accuracy is largely driven by the dominance of the healthy loan class (Class 0).

- **Precision (Class 1 - High-Risk Loan):** 0.87
Precision indicates that 87% of the loans predicted as high-risk were actually high-risk. There is still some misclassification of healthy loans as high-risk (false positives).

- **Recall (Class 1 - High-Risk Loan):** 1.00
The model achieved perfect recall for the minority class (Class 1). This means it correctly identified all high-risk loans, with no false negatives, which is crucial in risk prediction.

- **Precision (Class 0 - Healthy Loan):** 1.00
Precision for healthy loans is perfect, indicating that all loans predicted as healthy were truly healthy.

- **Recall (Class 0 - Healthy Loan):** 1.00
The model perfectly identified all healthy loans, with no false negatives.


# Summary

The machine learning model has performed exceptionally well in predicting the credit risk of loan applicants. The **accuracy score of 1.00** suggests that the model is performing well overall. However, given the class imbalance (many more healthy loans than high-risk loans), the **recall for Class 1** is particularly impressive, with **100% recall** meaning the model did not miss any high-risk loan.

The **precision for Class 1** is slightly lower at **0.87**, indicating that while the model is good at detecting high-risk loans, it also misclassifies some healthy loans as high-risk (false positives). This trade-off between precision and recall is common in credit risk modeling, where we prioritize recall to ensure that high-risk applicants are correctly identified.

# Recommendation:
Based on the results, I would recommend using this model for identifying high-risk loan applicants, especially because it does not miss any high-risk cases. While there is some room for improvement in terms of precision, the model’s strong recall makes it a reliable tool for flagging high-risk borrowers.

However, further fine-tuning or other advanced techniques such as **SMOTE** for better precision or experimenting with different models (e.g., decision trees or random forests) could be explored to further enhance performance. Additionally, testing the model with real-world data would provide a more accurate measure of its generalizability.
