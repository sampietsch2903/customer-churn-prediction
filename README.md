# Customer Churn Prediction

This project uses supervised machine learning to predict whether a customer will churn using the Telco dataset. 

## Dataset
- SourceL [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- 7,032 rows, 20 features (after cleaning)
- Target (dependent) variable: "Churn" (Yes/No)

## Tools Used
- Python
- pandas, numpy, scikit-learn, matplotlib, seaborn

## Workflow
1. Cleaned missing values and converted "TotalCharges" to numeric
2. Encoded categorical variables with one-hot encoding
3. Split dataset into training and testing sets
4. Trained 2 models:
   - Logistic Regression
   - Random Forest
5. Evaluated using confusion matrix, classification report, and ROC curve

## Key Results
- Logistic Regression slightly outperformed Random Forest on ROC AUC
- Both models showed strong separation between churn and non-churn classes

## ROC Curve
(![image](https://github.com/user-attachments/assets/a1681016-dee1-45dc-bfac-dfff4a45bfd8)

## Sample Output
Logistic Regression:
[[913 120]
 [161 213]]
              precision    recall  f1-score   support

           0       0.85      0.88      0.87      1033
           1       0.64      0.57      0.60       374

    accuracy                           0.80      1407
   macro avg       0.74      0.73      0.73      1407
weighted avg       0.79      0.80      0.80      1407

Random Forest:
[[917 116]
 [180 194]]
              precision    recall  f1-score   support

           0       0.84      0.89      0.86      1033
           1       0.63      0.52      0.57       374

    accuracy                           0.79      1407
   macro avg       0.73      0.70      0.71      1407
weighted avg       0.78      0.79      0.78      1407

