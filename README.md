Customer Churn Prediction – Machine Learning Project

This project focuses on predicting customer churn using various machine learning models. By analyzing customer data, the aim is to identify the factors contributing to churn and build predictive models that can help businesses improve retention strategies.

📌 Project Overview

Topic: Customer Churn Prediction

Dataset: Customer records including demographics, service usage, and billing information

Goal: Predict whether a customer will churn (leave the service)

Techniques used: Data preprocessing, exploratory data analysis, feature engineering, feature selection, and machine learning model evaluation

🛠️ Project Workflow
1. Data Preprocessing

Handled missing values (median for numerical, mode for categorical).

Dropped redundant/unnecessary columns.

Encoded categorical variables with LabelEncoder.

Treated outliers using the IQR method.

2. Exploratory Data Analysis (EDA)

Visualized distributions with histograms and boxplots.

Checked feature correlations using heatmaps.

Key insights:

Longer tenure → lower likelihood of churn

TotalCharges strongly correlates with tenure and monthly charges

3. Feature Engineering

New features were added to improve prediction power:

Monthly_Tenure_Ratio

Phone_Internet_Both

TotalCharges_Age_Ratio

Uses_Streaming

4. Feature Selection

Chi-Square Test

ExtraTreesClassifier feature importance

Sequential Feature Selection (SFS)

5. Machine Learning Models

Models trained & evaluated with cross-validation:

Logistic Regression (≈97.7% accuracy)

Decision Tree (≈99.8% accuracy)

Random Forest (≈99.8% accuracy)

K-Nearest Neighbors (≈93.8% accuracy)

Support Vector Classifier (≈94.2% accuracy)

6. Model Tuning

Used GridSearchCV to optimize hyperparameters.

Logistic Regression & KNN saw slight performance improvements.

├── data/                # Processed train/test datasets (CSV)
├── notebooks/           # Jupyter notebooks (EDA, preprocessing, modeling)
├── models/              # Saved ML models (Pickle files)
├── images/              # Plots & visualizations
├── README.md            # Project documentation

Author: Vaniprasad Vemuri
🎓 University of Messina – Bachelors in Data Analysis (21/22)

