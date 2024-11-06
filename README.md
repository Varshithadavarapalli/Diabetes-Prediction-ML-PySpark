# Diabetes-Prediction-ML-PySpark
Diabetes-Prediction-ML-PySpark


Project Overview

This project aims to predict and classify diabetes types and related conditions using machine learning models. We utilized PySpark for distributed data processing and multiple machine learning models to evaluate their effectiveness in diabetes classification tasks. The focus was on comparing various metrics, such as accuracy, precision, recall, F1 score, and specificity, to identify the model best suited for the dataset.

Project Objectives

The main goal of this project is to utilize machine learning models to predict diabetes categories accurately. Each model’s performance was compared to identify strengths and areas for improvement. Key objectives include:

Preprocessing data for quality and consistency.
Implementing and comparing models to determine the most effective approach.
Analyzing metrics like accuracy, precision, recall, F1 score, and specificity.

Dataset and Preprocessing
We used a structured health dataset for diabetes prediction. Key preprocessing steps included:

Handling Missing Values: Imputed missing values using median values.
Column Name Normalization: Removed spaces from column names for ease of reference.
Label Encoding: Converted categorical labels to numeric format.


Model Implementations
Three models were evaluated:

Random Forest (Varshitha): Achieved high accuracy, precision, and specificity, making it the top-performing model.
K-Nearest Neighbors (KNN) (Saketha): Converted the dataset to Pandas for Scikit-Learn compatibility due to Spark’s lack of native KNN support.
Logistic Regression (Karunakar): A linear approach that provided moderate accuracy and interpretability.

Code Explanation
Setting up Spark Session and Loading Data: Initialized a Spark session for data processing and loaded the dataset.
Data Preprocessing: Cleaned column names, encoded the target variable, and handled missing values.
Feature Vector Assembly: Assembled numeric features into a single vector for compatibility with PySpark ML models.
Model Training and Evaluation: Split data into training and testing sets (70/30) and evaluated each model based on performance metrics.


Python Packages Used
PySpark: For data handling and machine learning model implementation.
Scikit-Learn: For K-Nearest Neighbors model.
Pandas: To convert PySpark DataFrames to Pandas for compatibility with Scikit-Learn’s KNN implementation.
Conclusion
Each model had unique strengths and was best suited for specific use cases:

Random Forest: Optimal for large, complex datasets.
K-Nearest Neighbors: Effective for closely clustered data but resource-intensive.
Logistic Regression: Quick, interpretable results on simpler datasets.
