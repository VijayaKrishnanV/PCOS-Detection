# PCOS-Detection

This Python script implements a machine learning workflow for diagnosing Polycystic Ovary Syndrome (PCOS) using a Random Forest Classifier. The script performs data loading, preprocessing, model training, evaluation, and user interaction. Below is an outline of its key components and functionality:

Library Imports:

Essential libraries for data manipulation (pandas, numpy), machine learning (sklearn), and visualization (matplotlib, seaborn) are imported.


Data Loading:

Two datasets are loaded: one containing data for patients with PCOS and another for patients without PCOS. These datasets are merged based on a common identifier (Patient File No.).


Data Preprocessing:

Unnecessary columns are dropped.
Data types are corrected, converting numeric values stored as strings into appropriate numeric formats.
Column names are cleaned of extra spaces.
Missing values in the dataset are handled using median imputation.


Exploratory Data Analysis (EDA):

Basic statistical details of the dataset are examined.
A correlation matrix is computed and visualized to understand the relationships between features and the target variable (PCOS (Y/N)).
Heatmaps of feature correlations are plotted to identify significant features.


Feature and Target Assignment:

Features (X) and the target variable (y) are separated. The target variable is the presence or absence of PCOS.


Data Splitting:

The dataset is split into training and test sets using a 70-30 split.


Model Training and Tuning:

A Random Forest Classifier is initially trained and evaluated.
GridSearchCV is used to find the best hyperparameters for the model.
The model is retrained with the best parameters found from GridSearchCV.


Model Evaluation:

The final model is tested on the test set.
Performance metrics including accuracy, classification report, and confusion matrix are computed and visualized.


User Input and Prediction:

The script takes user input for various health metrics and creates a new data point.
The trained model makes a prediction based on the user input and provides an output indicating the likelihood of PCOS.


Model Performance Visualization:

A bar chart is plotted to compare the accuracy of the model before and after hyperparameter tuning.
