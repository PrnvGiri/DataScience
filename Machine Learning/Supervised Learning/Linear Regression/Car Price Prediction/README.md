# Car Price Prediction

## Overview
This project involves building a multiple linear regression model to predict the price of cars based on various independent features. The analysis determines which factors significantly affect the price and provides a predictive model for pricing strategy.

## Dataset
The dataset used for this project is `scrap price.csv`. It contains 205 entries with 26 columns, including:
- **Target Variable**: `price`
- **Features**: `symboling`, `wheelbase`, `enginesize`, `horsepower`, `peakrpm`, `citympg`, `highwaympg`, etc.

## Technologies Used
- **Python**: Core programming language.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib & Seaborn**: For data visualization.
- **Scikit-learn**: For implementing the Linear Regression model.

## Project Structure
- `Linear_regression_car_price_prediction.ipynb`: The Jupyter Notebook containing the data analysis, visualization, and model implementation.
- `scrap price.csv`: The dataset used for training and testing the model.

## How to Run
1. Ensure you have Python and Jupyter Notebook installed.
2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Open the notebook `Linear_regression_car_price_prediction.ipynb` and execute the cells.

## Analysis
The notebook includes:
- Data Loading and Cleaning
- Exploratory Data Analysis (EDA)
- Feature Selection
- Model Building using Linear Regression
- Model Evaluation
