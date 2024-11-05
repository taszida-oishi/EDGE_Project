# Housing Price Prediction

This project focuses on predicting housing prices using a range of machine learning models, including Linear Regression, Decision Trees, and XGBoost, integrated into a Voting Regressor. The Jupyter Notebook processes housing data, encodes categorical features, and visualizes key relationships, ultimately training and evaluating multiple models to enhance prediction accuracy and address the challenges posed by multicollinearity among features.

## Table of Contents

- [Housing Price Prediction](#housing-price-prediction)
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Objectives](#objectives)
- [Requirements](#requirements)
- [Code Description](#code-description)
- [Results](#results)
- [Contribution](#contribution)

## Project Overview

This project aims to predict housing prices based on various features such as house area, number of bedrooms, furnishing status, proximity to main roads, and more. The dataset, while small, presents a challenge due to the strong multicollinearity among the features, making it essential to develop a robust predictive model.

## Dataset Description

The dataset consists of several key features that impact housing prices, including but not limited to:

- **House Area:** The total area of the house in square feet.
- **Bedrooms:** The number of bedrooms in the house.
- **Furnished:** Indicates whether the house is furnished (yes/no).
- **Nearness to Main Road:** A binary variable indicating the proximity of the house to the main road.

The complexity of this dataset arises from the relationships between these features, requiring careful feature selection and preprocessing to build an effective model.

## Objectives

- Analyze the dataset to understand feature relationships and distributions.
- Handle multicollinearity to improve model performance.
- Build and evaluate predictive models to accurately forecast housing prices.

## Requirements

Make sure you have the following libraries installed:

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- xgboost

## Code Description

The Jupyter Notebook contains the following key steps:

1. **Data Loading and Preprocessing:**
   - Load the dataset and perform initial exploration.
   - Encode categorical variables using `LabelEncoder` and `OrdinalEncoder`.
   - Check for duplicates and missing values.

2. **Data Visualization:**
   - Visualize the distribution of housing prices and boxplots to identify outliers.
   - Generate a correlation heatmap to explore feature relationships.

3. **Model Training:**
   - Split the dataset into training and testing sets.
   - Scale the features using `StandardScaler`.
   - Train multiple regression models, including Linear Regression, Decision Tree, Random Forest, and XGBoost, using cross-validation to evaluate their performance.

4. **Voting Regressor:**
   - Combine predictions from different models using a Voting Regressor and evaluate its performance using R² scores.

5. **Hyperparameter Tuning:**
   - Experiment with different weights for the Voting Regressor to optimize performance.

## Results

The final model's performance is evaluated using R² scores, and predictions are visualized to compare actual prices versus predicted prices.

## Contribution

Feel free to contribute to this project by submitting a pull request. Any improvements or suggestions are welcome!

