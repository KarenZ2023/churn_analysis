# Customer Churn Analysis

This repository contains code and data for analyzing customer churn for a travel agency.

## Files

- `ChurnAnalysis.ipynb`: Jupyter Notebook containing Python code for churn analysis.
- `Customer_Travel_EDA.html`: HTML output of data profiling using ydata_profiling.
- `Kaggle_Customertravel.csv`: Dataset for churn analysis obtained from Kaggle.

## Problem Statement

The goal of this project is to predict customer churn for a travel agency based on various indicators, such as age, income, whether lodgings are booked, etc.

## Dataset

The dataset used in this analysis is obtained from Kaggle: [Tour Travels Customer Churn Prediction](https://www.kaggle.com/datasets/tejashvi14/tour-travels-customer-churn-prediction).

## Methods

1. **Data Exploration using ydata_profiling**
   - 23.48% customers churn
   - 76.51% loyal customers

2. **Data Wrangling**
   - Remove missing data: Remove customers where 'FrequentFlyler' is 'No Record', and 60 entries removed
   - Encode categorical data into numeric values

3. **Model Building**
   - Use SMOTE to correct for imbalanced data
   - Build a pipeline to test various models (logistic regression, random forest, KNN, Adaboost Classifier)

4. **Model Evaluation**
   - Choose the best model based on accuracy

## Takeaways

All the models performed similarly and have an accuracy ~0.78 to ~0.85. The model with the highest accuracy is the random forest model with an accuracy of 0.85. Random Forest likely performed better due to its ensemble nature, which combines multiple decision trees to reduce overfitting and capture complex relationships in the data more effectively. Additionally, its ability to handle non-linearity and interactions between features, along with providing feature importance scores, contributed to its superior performance in this scenario.

With the ability to classify customers at risk of churning, the business can implement targeted retention strategies. These include personalized interventions, proactive engagement initiatives, and tailored offers aimed at incentivizing at-risk customers to stay loyal.

