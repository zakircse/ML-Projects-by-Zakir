# 🪙 Gold Price Prediction Using Machine Learning
## 📘 Overview

This project builds a machine learning model to predict gold prices based on various market indicators. Using a historical dataset of gold prices and related financial variables, it applies data preprocessing, exploratory analysis, and a Random Forest Regressor to forecast the value of gold (denoted by GLD).

The notebook demonstrates a complete ML pipeline — from data exploration to model evaluation — aimed at understanding the relationships between economic indicators and gold pricing trends.

## 📊 Dataset

The dataset used in this project (gold_price_data.csv Link: https://www.kaggle.com/datasets/altruistdelhite04/gold-price-data) contains historical financial data with the following attributes:

Date – Time period of observation

SPX – S&P 500 Index

USO – United States Oil Fund prices

SLV – Silver prices

EUR/USD – Euro-to-Dollar exchange rate

GLD – Gold ETF closing price (Target variable)

The dataset is clean and well-structured, with no missing values. Descriptive statistics and correlation analysis were used to understand variable interactions.

## 🧹 Data Preprocessing

Feature Selection: Removed non-numeric columns (Date) to focus on numerical predictors.

Exploratory Analysis:

Heatmap: Visualized correlations between features and gold price.

Distribution Plot: Checked the target variable’s distribution for normality.

Feature & Target Split:

X → independent features (SPX, USO, SLV, EUR/USD)

y → dependent variable (GLD)

Train-Test Split: 80% training, 20% testing (random state = 2)

## 🤖 Model Implementation

A Random Forest Regressor was chosen for its robustness and ability to capture non-linear relationships in financial data.

Algorithm: Random Forest Regressor (100 estimators)

Framework: Scikit-learn

Training: Fit on training data

Prediction: Performed on test set

## 📈 Model Evaluation

Metric Used: R² Score (Coefficient of Determination)

The model achieved a high R² value, indicating strong predictive performance and minimal overfitting.

Visualization:

Plotted Actual vs Predicted gold prices to visually assess accuracy.

The two lines nearly overlap, confirming the model’s reliability.
