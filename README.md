# Breast Cancer Classification using Random Forest

## Project Overview

This project implements an end-to-end machine learning pipeline for breast cancer classification using the Breast Cancer Wisconsin dataset.

The system performs data loading, preprocessing, missing-value handling, train-test splitting, model training, prediction, evaluation, visualization, and model persistence using Python and Scikit-learn.

## Objectives

- Load and preprocess breast cancer dataset
- Handle missing values using imputation
- Train a Random Forest classification model
- Evaluate model performance using classification metrics
- Generate a confusion matrix
- Analyze feature importance
- Save and reload the trained machine learning pipeline

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Joblib

## Machine Learning Algorithm

### Random Forest Classifier

The project uses a Random Forest Classifier with:

- 300 decision trees
- Random state: 42
- Parallel processing using all available CPU cores

The model is integrated with a Scikit-learn Pipeline containing a median-based SimpleImputer for handling missing values.

## Dataset

The project uses the Breast Cancer Wisconsin dataset.

The dataset contains features including:

- Clump Thickness
- Uniformity of Cell Size
- Uniformity of Cell Shape
- Marginal Adhesion
- Single Epithelial Cell Size
- Bare Nuclei
- Bland Chromatin
- Normal Nucleoli
- Mitoses

The target variable is:

- CancerType

Where:
- `2` = Benign
- `4` = Malignant

## Project Workflow

```text
Raw Dataset
     ↓
Data Loading
     ↓
Add Dataset Headers
     ↓
Missing Value Handling
     ↓
Feature Selection
     ↓
Train-Test Split
     ↓
SimpleImputer
     ↓
Random Forest Classifier
     ↓
Model Training
     ↓
Prediction
     ↓
Model Evaluation
     ↓
Feature Importance
     ↓
Save Trained Model
     ↓
Load Model & Test Prediction
