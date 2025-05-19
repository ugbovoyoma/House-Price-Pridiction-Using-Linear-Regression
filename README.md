# House Price Pridiction Using Linear Regression
This repository contains a **Linear Regression model** that predicts house prices based on the square footage, number of bedrooms, and bathrooms.

## 📌 Task
The goal is to **predict house prices** using the following features:
- Square footage of the house
- Number of bedrooms
- Number of bathrooms
## Data Preparation

Read the dataset using Pandas.

Checked for missing values and duplicate rows.

Verified data types

Created a new dataset using only relevant features.

##  Model Training

Split the dataset into training and testing sets using Scikit-learn.

Implemented a Linear Regression model to predict house prices.

Extracted model coefficients to interpret feature importance.

# **Result And Findings**
After implementing the linear regression model using the selected features (GrLivArea, BedroomAbvGr, FullBath, and HalfBath), the model was trained and evaluated using an 80-20 train-test split. The performance of the model was assessed using Mean Squared Error (MSE) as the evaluation metric.

**Mean Squared Error (MSE):** 
The model achieved an MSE of 2810942965.22, indicating the average squared difference between the predicted and actual sale prices. This value reflects how well the model fits the test data.

**Feature Importance:** 
Among the features used, GrLivArea (above ground living area in square feet) appeared to have the most significant impact on predicting house prices. This is consistent with domain knowledge, as larger homes generally tend to have higher values.



# **Model Interpretation:**

Since linear regression provides a straightforward interpretation of coefficients, we observed that the coefficients for FullBath and BedroomAbvGr also positively influenced the predicted sale price, although not as strongly as GrLivArea. HalfBath had a smaller but still positive contribution.

# **Model Limitations:**

The model is relatively simple and only considers four features. Many other features from the dataset (e.g., overall quality, neighborhood, garage area) were excluded because they were not part of the instruction given and could improve prediction accuracy.

Linear regression assumes a linear relationship between the input features and the target variable. In reality, the relationship between house features and price may be nonlinear and more complex.
