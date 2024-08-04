# CODETECH-Task1
- **Name**: KAVADE VAMSHI MOHAN
- **Company**: CODETECH IT SOLUTIONS
- **ID**: CT08DS4246
- **Domain**: MACHINE LEARNING
- **Duration**: July to August 2024
- **Mentor**: Muzammil Ahmed
# House Price Prediction Model

## Overview

This project presents a machine learning model designed to predict house prices based on various attributes of a property. The model utilizes a dataset containing information such as location, square footage, number of bedrooms, and other relevant features to estimate the price of a house. The goal of this project is to build a predictive model that can assist homeowners, real estate professionals, and potential buyers in making informed decisions by providing accurate price predictions.

## Dataset

The dataset used in this project contains several features that are commonly associated with house pricing. These features include:

- **Square Feet**: The total area of the house in square feet.
- **Number of Bedrooms**: The total number of bedrooms in the house.
- **Number of Bathrooms**: The total number of bathrooms in the house.
- **Number of Floors**: The number of floors in the house.
- **Year Built**: The year the house was originally built.
- **Year Renovated**: The year the house was last renovated, if applicable.
- **Location**: The city where the house is located.
- **Price**: The target variable, representing the price of the house.

The dataset is preprocessed to handle missing values, categorical variables, and any inconsistencies before being used to train the model.

## Methodology

The project follows a standard machine learning workflow:

### 1. Data Preprocessing

- **Data Cleaning**: Missing values are handled, either by imputing with appropriate values or by removing rows/columns where necessary.
- **Feature Engineering**: New features may be derived from existing ones to enhance the predictive power of the model.
- **Encoding Categorical Variables**: Categorical variables, such as 'Location', are converted into numerical formats using techniques like one-hot encoding or label encoding.
- **Feature Scaling**: Numerical features are scaled to ensure they contribute equally to the model training process.

### 2. Exploratory Data Analysis (EDA)

EDA is conducted to understand the distribution of features, detect outliers, and explore the relationships between the features and the target variable (Price). Visualization tools such as histograms, scatter plots, and correlation matrices are used in this phase to gain insights from the data.

### 3. Model Selection and Training

The model selection process involves trying different algorithms to find the one that best fits the data. In this project, a **Linear Regression** model is primarily used due to its simplicity and interpretability. However, other models like **Decision Trees**, **Random Forests**, and **Gradient Boosting** may also be explored depending on the project’s requirements.

The dataset is split into training and testing sets, with the training set used to train the model and the testing set used to evaluate its performance. Cross-validation techniques are also employed to ensure the model generalizes well to unseen data.

### 4. Model Evaluation

The model’s performance is evaluated using various metrics, including:

- **Mean Absolute Error (MAE)**: Measures the average magnitude of errors in predictions.
- **Mean Squared Error (MSE)**: Measures the average squared difference between predicted and actual values.
- **Root Mean Squared Error (RMSE)**: The square root of MSE, providing a measure of error in the same units as the target variable.
- **R-squared**: Indicates the proportion of variance in the target variable that is predictable from the features.

These metrics help in understanding how well the model is performing and where improvements can be made.

### 5. Model Deployment

Once a satisfactory model is developed, it can be deployed for real-time predictions. This project demonstrates how to deploy the trained model using a simple web API, built using **Flask**. Users can input new house data to get price predictions via the API.

## Results

The model achieves reasonable accuracy in predicting house prices, with evaluation metrics such as MAE, MSE, and RMSE within acceptable ranges. These results indicate the model's capability to generalize well to unseen data and provide useful predictions in real-world scenarios.
