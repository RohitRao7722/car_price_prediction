# Car Price Prediction


This project is designed to predict the prices of used cars based on various features such as the car’s company, model, year of manufacture, kilometers driven, fuel type, and more. The goal of the project is to build a machine learning model that can predict the price of a car given these features.

## Project Overview

The car price prediction model takes a dataset of used cars, performs data cleaning and preprocessing, and trains a model to predict car prices. The dataset includes various columns such as the car’s name, company, year, kilometers driven, fuel type, and price.

## Features

- **Name:** Name of the car model
- **Company:** Manufacturer of the car
- **Year:** Year of manufacture
- **Kilometers Driven:** Number of kilometers the car has been driven
- **Fuel Type:** Type of fuel used by the car (Petrol, Diesel, CNG, etc.)
- **Price:** Price of the car (Target variable)

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/car-price-prediction.git
   ```

2. **Install the required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

## Project Workflow

1. **Data Cleaning:**
   - Handle missing values.
   - Convert categorical variables (such as fuel_type) into numerical values using one-hot encoding.
   - Filter out outliers in the target variable `Price` and other columns like `kms_driven` to ensure better model performance.

2. **Feature Engineering:**
   - Apply one-hot encoding to categorical variables like `name`, `company`, and `fuel_type`.
   - Add new features like the age of the car (calculated as 2024 - year) to improve the model's predictive power.

3. **Model Building:**
   - Use Linear Regression as the baseline model for predicting the car price.
   - Perform cross-validation to assess the model’s performance on different data splits.

4. **Evaluation:**
   - Evaluate the model’s performance using metrics like R-squared and Mean Squared Error (MSE).
   - Perform a final evaluation of the test data to determine the model's ability to generalize.

## Files and Directories

- **data/:** Contains the dataset used for training and testing the model.
- **notebooks/:** Jupyter
