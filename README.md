# Berkeley-Capstone

Credit Card Fraud Detection – EDA & Baseline Modeling

Project Overview
This project explores a dataset of credit card transactions to detect fraudulent activity using machine learning. The focus of this phase is on exploratory data analysis (EDA) and developing a baseline classification model to predict fraud. This work sets the foundation for further model improvements in the next module.
Dataset Source: Kaggle - Credit Card Fraud Detection 2023

________________________________________
Research Question
How can machine learning be used to accurately classify fraudulent credit card transactions based on anonymized transaction features?
________________________________________
Dataset Summary
•	Total Records: 568,630
•	Features: 31
o	Anonymized variables (V1 to V28)
o	Amount, id, and Class (target)
•	Missing Values: None
•	Duplicates: None found
•	Class Distribution:
o	Fraudulent: 50%
o	Non-Fraudulent: 50%
________________________________________
Key Findings from EDA
•	Features V4 and V11 are most positively correlated with fraud.
•	Features V14 and V12 are most negatively correlated with fraud.
•	The dataset appears balanced, making traditional evaluation metrics reliable without re-balancing.
•	No significant outliers in scaled Amount by class.
Top 5 Positively Correlated Features with Fraud:
•	V4 (0.74), V11 (0.72), V2 (0.49), V19 (0.24), V27 (0.21)
Top 5 Negatively Correlated Features with Fraud:
•	V14 (-0.81), V12 (-0.77), V10 (-0.68), V9 (-0.59), V16 (-0.57)
________________________________________
Visualizations
•	Class Distribution Plot
•	Correlation Heatmap of Top Features
•	Boxplot of Scaled Amount by Class
•	Pairplot of Highly Correlated Features
•	ROC Curve for Model Evaluation
________________________________________
Baseline Model
Model Used: Logistic Regression (with balanced class weight)
Performance:
•	ROC-AUC Score: 0.9935
•	Confusion Matrix:
•	[[55591  1272]
•	 [ 2715 54148]]
•	Classification Report:
o	Precision (Fraud): 0.98
o	Recall (Fraud): 0.95
o	F1-Score (Fraud): 0.96
________________________________________
Methodology Update
There have been no changes to the dataset or overall methodology update since earlier

________________________________________
Next Steps
•	Implement additional models (Random Forest, XGBoost)
•	Conduct hyperparameter tuning
•	Perform feature importance analysis (e.g., SHAP values)
•	Improve model explainability and presentation


