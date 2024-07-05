# Flagging Loans Project

## Overview

This project aims to build a model to predict loan defaults using a dataset containing information on repeated loans from current clients. The main goal is to predict the value of the target variable `bad_flag` and analyze the expected default rate at different approval levels.

## Project Structure

The project is divided into several phases:

1. Data Import and Preprocessing
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
4. Algorithm Selection
5. Model Evaluation and Feature Importance

## Key Features

- Utilizes various machine learning algorithms for classification
- Addresses class imbalance using undersampling and SMOTE
- Performs cross-validation to ensure model generalization
- Visualizes model performance using ROC and Precision-Recall curves
- Analyzes feature importance

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn (Version `1.1`)
- imbalanced-learn (imblearn) (Version `0.12.2`)
- yellowbrick

## Main Steps

1. Import and preprocess the dataset
2. Perform EDA to understand data distributions and correlations
3. Engineer new features and handle categorical variables
4. Compare multiple classification algorithms
5. Address class imbalance using undersampling and SMOTE
6. Evaluate model performance using cross-validation, learning curves, and ROC/PR curves
7. Analyze feature importance

## Model Selection

The project evaluates several classifiers, including:

- SGDClassifier
- KNeighborsClassifier
- LogisticRegression
- BaggingClassifier
- GaussianNB
- RandomForestClassifier
- ExtraTreesClassifier

The ExtraTreesClassifier showed the best performance after addressing class imbalance.

## Results

- The final model (ExtraTreesClassifier) achieved high performance metrics, with an AUC of 0.98 and an Average Precision of 0.98.
- The most important features for predicting loan defaults were identified and visualized.
