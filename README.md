# Loan_Status_Classifier
Loan Approval Prediction Model 🏦
This project uses a machine learning model to predict the likelihood of a loan application being approved. The goal is to automate and streamline the initial screening process by classifying new applications as either "approved" or "rejected" based on key applicant details.

Model Used: Random Forest Classifier 🌲
The core of this project is a Random Forest Classifier. This powerful and highly accurate model is an ensemble learning method, meaning it combines the predictions of many individual decision trees to make a single, more reliable forecast.

How It Works: Instead of relying on a single, potentially biased decision tree, the Random Forest builds a "forest" of numerous trees. Each tree is trained on a random subset of the data and features. When a new loan application is processed, each tree in the forest casts a "vote" on whether to approve or reject the loan. The final prediction is the class that receives the majority of votes from all the trees.

Why It's a Good Choice: The Random Forest's strength lies in its ability to handle complex, non-linear data and its inherent resistance to overfitting. This makes it a robust and dependable choice for predicting outcomes like loan approval.

Model Performance
The model's performance was evaluated on a held-out test set, achieving an impressive accuracy of approximately 86%. This means that the model correctly predicts the outcome (approved or rejected) for 86 out of every 100 new loan applications.

Input Features
The model requires 11 key features as input to make a prediction. These features must be provided in a specific order and in numerical format.

The input order is:

Gender (e.g., 0 for Male, 1 for Female)

Married (e.g., 0 for No, 1 for Yes)

Dependents (Number of dependents)

Education (e.g., 0 for Not Graduate, 1 for Graduate)

Self_Employed (e.g., 0 for No, 1 for Yes)

ApplicantIncome

CoapplicantIncome

LoanAmount

Loan_Amount_Term

Credit_History (e.g., 0 for Bad, 1 for Good)

Property_Area (e.g., 0 for Rural, 1 for Semiurban, 2 for Urban)

How to Test the Model
To test the model, you can provide the 11 numerical feature values as a single, space-separated string.

Example Input:
0 1 0 1 0 8000 1500 200 360 1 1

This input would represent a male, married, graduate applicant with a good credit history and a significant income.
