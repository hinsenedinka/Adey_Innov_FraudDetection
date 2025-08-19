# Fraud Detection Project
📜 Overview
This project aims to build and evaluate machine learning models for detecting fraudulent e-commerce and credit card transactions for Adey Innovations Inc. It addresses the core challenge of class imbalance in two distinct datasets and uses advanced techniques like feature engineering and model explainability to deliver an effective and interpretable solution.

📊 Datasets
The project utilizes three datasets:

Fraud_Data.csv: E-commerce transaction data with features like purchase_time, purchase_value, source, and a target variable class.

IpAddress_to_Country.csv: A lookup table to map IP addresses from Fraud_Data.csv to geographic locations.

creditcard.csv: Anonymized credit card transaction data with PCA-transformed features (V1 to V28), Amount, and a target variable Class.

Critical Challenge: Both fraud datasets suffer from severe class imbalance, meaning fraudulent cases are extremely rare.

🚀 Key Tasks
The project is structured into three main tasks:

***Data Analysis & Preprocessing***
Cleaning: Handle missing values and duplicates.

Feature Engineering: Create new features such as time_since_signup and transaction frequency.

Geolocation: Merge e-commerce data with the IP address country data.

Handling Imbalance: Apply techniques like SMOTE or Random Undersampling on the training data to address class imbalance.

Transformation: Normalize numerical features and encode categorical ones.

***Model Building & Training***
Model Selection: Compare a baseline Logistic Regression model against a powerful ensemble model, such as Random Forest or XGBoost.

Evaluation: Train and evaluate models using metrics suitable for imbalanced data, including F1-Score and AUC-PR (Area Under the Precision-Recall Curve), to justify the "best" model choice.

***Model Explainability***
SHAP Analysis: Use SHAP (Shapley Additive exPlanations) to interpret the predictions of the best-performing model.

Insights: Generate and analyze SHAP plots (e.g., Summary and Force plots) to identify the key features driving fraud detection. The final report will explain what these plots reveal about the model's decision-making process.