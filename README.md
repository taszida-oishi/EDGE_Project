Housing Price Prediction
Project Overview
This project aims to predict housing prices based on various features such as house area, number of bedrooms, furnishing status, proximity to main roads, and more. The dataset, while small, presents a challenge due to the strong multicollinearity among the features, making it essential to develop a robust predictive model.
Dataset Description
The dataset consists of several key features that impact housing prices, including but not limited to:
•	House Area: The total area of the house in square feet.
•	Bedrooms: The number of bedrooms in the house.
•	Furnished: Indicates whether the house is furnished (yes/no).
•	Nearness to Main Road: A binary variable indicating the proximity of the house to the main road.
The complexity of this dataset arises from the relationships between these features, requiring careful feature selection and preprocessing to build an effective model.
Objectives
•	Analyze the dataset to understand feature relationships and distributions.
•	Handle multicollinearity to improve model performance.
•	Build and evaluate predictive models to accurately forecast housing prices.
Requirements
Make sure you have the following libraries installed:
•	pandas
•	numpy
•	scikit-learn
•	matplotlib
•	seaborn
•	xgboost
Code Description
The Jupyter Notebook contains the following key steps:
1.	Data Loading and Preprocessing:
o	Load the dataset and perform initial exploration.
o	Encode categorical variables using LabelEncoder and OrdinalEncoder.
o	Check for duplicates and missing values.
2.	Data Visualization:
o	Visualize the distribution of housing prices and boxplots to identify outliers.
o	Generate a correlation heatmap to explore feature relationships.
3.	Model Training:
o	Split the dataset into training and testing sets.
o	Scale the features using StandardScaler.
o	Train multiple regression models, including Linear Regression, Decision Tree, Random Forest, and XGBoost, using cross-validation to evaluate their performance.
4.	Voting Regressor:
o	Combine predictions from different models using a Voting Regressor and evaluate its performance using R² scores.
5.	Hyperparameter Tuning:
o	Experiment with different weights for the Voting Regressor to optimize performance.
Results
The final model's performance is evaluated using R² scores, and predictions are visualized to compare actual prices versus predicted prices.
Contribution
Feel free to contribute to this project by submitting a pull request. Any improvements or suggestions are welcome!
