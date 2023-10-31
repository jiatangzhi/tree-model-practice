# Tree Model Practice

## Overview

This repository contains code and documentation for Homework 3, which involves data preprocessing, model training, and tuning for a regression task. The goal is to predict a quantitative outcome using various predictor variables from a toy dataset. We will explore different approaches for handling categorical data, train several machine learning models, and evaluate their performance.

## Steps

### Step 1: Reading Assignment

Before diving into the practical aspects, it is essential to understand the theoretical foundations. Read Section 8.2 (pp 343-354) of our textbook "An Introduction to Statistical Learning - with Applications in Python."

### Step 2: Handling Categorical Data

#### One-Hot Encoding (OHE)

a. **Explanation:** One-Hot Encoding (OHE) is a method for converting categorical variables into binary matrix representations. It represents each unique label as a separate binary column, where each column corresponds to the presence or absence of a specific category.

Pros of OHE:
- Simple and easy to implement.
- Works well with algorithms that assume no ordinal relationship among categories.

Cons of OHE:
- Can lead to high dimensionality in the dataset, especially with a large number of unique labels.
- Ignores ordinal relationships among categories.

b. **Application:** Apply One-Hot Encoding to all categorical variables in the dataset.

### Step 3: Training Models with Default Parameters

1. **Linear Regression Model:** Train a Linear Regression model using the dataset.
2. **Decision Tree Regressor:** Train a Decision Tree Regressor model.
3. **Random Forest Regressor:** Train a Random Forest Regressor model.

Evaluate these models using appropriate metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R2) on a test set.

### Step 4: Tuning Models

Select the best-performing model from the previous step and perform sequential tuning on at least two hyperparameters. Tune one parameter at a time and plot the performance against each parameter value.

#### Example Tuning:

- Tune `n_estimators` for Random Forest.
- Tune `max_depth` for Random Forest.

a. **Print the values of the best-tuned parameters.**

b. **Give the score of the tuned model on the test set.**

### Step 5: Advanced Hyperparameter Tuning

Use GridSearchCV or RandomizedSearchCV from sklearn to tune two or more hyperparameters simultaneously. Print the best parameters and save the best model. Evaluate the model's score on the test set.

## Conclusion

By following these steps, you will gain practical experience in data preprocessing, model training, and hyperparameter tuning for regression tasks. Experiment with different approaches and hyperparameters to improve your understanding of machine learning techniques. 
