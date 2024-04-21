# Home Credit Default Risk Analysis

This repository contains a Jupyter Notebook for the Kaggle competition, "Home Credit Default Risk". The goal of the competition is to predict how capable each applicant is of repaying a loan.

## Overview

The notebook includes an extensive exploratory data analysis, preprocessing, feature engineering, and the development of several machine learning models to predict the likelihood of loan repayment.

## Data

The data used in this project is from the [Home Credit Default Risk Kaggle Competition](https://www.kaggle.com/c/home-credit-default-risk). It consists of several files which include the main application training and test datasets, as well as various supplementary datasets.

## Contents

The notebook is structured as follows:

1. **Import Datasets**: Load the main training and test datasets.
2. **Data Preparation**: Data cleaning, handling missing values, label encoding, one-hot encoding, and downsampling data.
3. **Model Development**: Development of Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting models.
4. **Model Evaluation**: Evaluation of the Gradient Boosting model on the test dataset using ROC-AUC as the performance metric.

## Models Developed

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting

The Gradient Boosting model showed the best performance on the validation set.
