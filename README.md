# PCOS-Detection
Engineered a machine learning solution using Random Forest to identify Polycystic Ovary Syndrome (PCOS) from demographic and clinical parameters, achieving significant accuracy and enhancing personalized healthcare by pinpointing individuals at risk.

PCOS Detection Using Machine Learning
This project utilizes machine learning techniques to predict the likelihood of Polycystic Ovary Syndrome (PCOS) based on various patient parameters. The steps involved are as follows:

Data Integration and Preprocessing:

Data from two sources (patients with and without infertility) are merged based on patient identifiers.
Columns are cleaned, and data types are adjusted for numerical analysis.
Exploratory Data Analysis:

Statistical summaries and correlation matrices are generated to understand relationships between features and PCOS diagnosis.
Model Building:

A RandomForestClassifier is trained to predict PCOS status.
The model is initially evaluated for accuracy.
Model Tuning:

GridSearchCV is employed to optimize the RandomForestClassifier by testing various hyperparameters.
The model is retrained using the best parameters identified.
Model Evaluation:

Performance metrics such as accuracy, confusion matrix, and classification report are computed to assess the model's predictive capability.
Prediction Tool:

An interactive tool allows users to input personal health metrics to receive a prediction regarding PCOS diagnosis.
Visualization:

Visual representations, such as bar charts, compare model accuracy before and after tuning.
This project provides a comprehensive pipeline for detecting PCOS using machine learning, aiming to assist healthcare professionals in diagnosis and treatment planning.

