# Linear Regression Model for Insurance Claim Prediction

This repository contains a linear regression model built to predict insurance claim amounts (`charges`) using a dataset of insurance information. The dataset includes features such as age, sex, BMI, number of children, smoking status, past consultations, number of steps, hospital expenditure, number of past hospitalizations, annual salary, and region.

## Dataset

The dataset used is `insurance_data.csv`, which includes the following columns:

-   `age`: Age of the insured.
-   `sex`: Gender of the insured (male/female).
-   `bmi`: Body mass index of the insured.
-   `children`: Number of children covered by the insurance.
-   `smoker`: Smoking status of the insured (yes/no).
-   `Claim_Amount`: Claim Amount.
-   `past_consultations`: Number of past medical consultations.
-   `num_of_steps`: Number of steps taken by the insured.
-   `Hospital_expenditure`: Hospital expenditure.
-   `NUmber_of_past_hospitalizations`: Number of past hospitalizations.
-   `Anual_Salary`: Annual salary of the insured.
-   `region`: Region of residence of the insured.
-   `charges`: Insurance claim amount (target variable).

## Project Structure
-   `insurance_data.csv`: The dataset used for the project.
-   `Linear_Regression_Insurance_Claims.ipynb`: Jupyter Notebook containing the code for EDA, multicollinearity handling (VIF), and linear regression model implementation.
-   `README.md`: This file.

## Implementation Details

The `Linear_Regression_Insurance_Claims.ipynb` notebook implements the following steps:

1.  **Data Loading and Exploration (EDA):**
    -      Loading the `insurance_data.csv` dataset.
    -      Performing basic exploratory data analysis (EDA) to understand the data distribution and relationships between variables.
    -      Visualizing the data using plots and charts.
    -   Handling categorical variables using one hot encoding.
2.  **Multicollinearity Handling (VIF):**
    -      Calculating the Variance Inflation Factor (VIF) to detect multicollinearity among the independent variables.
    -      Removing highly correlated variables based on the VIF scores to improve the model's performance.
3.  **Linear Regression Model:**
    -      Splitting the data into training and testing sets.
    -      Training a linear regression model using the training data.
    -      Evaluating the model's performance using metrics such as R-squared and Mean Squared Error (MSE).
4.  **Model Evaluation:**
    -   Visualizing the predicted vs actual values.
    -   Printing the R-squared and MSE values.
5.  **Model Improvements**
    -   Removing Outliers.
    -   Feature Scaling.

## Libraries Used

-   `pandas`
-   `numpy`
-   `matplotlib`
-   `seaborn`
-   `sklearn`
-   `statsmodels`

## How to Run

1.  Clone this repository to your local machine.
2.  Ensure you have the required libraries installed. You can install them using pip:

    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
    ```

3.  Open and run the `Linear_Regression_Insurance_Claims.ipynb` Jupyter Notebook.

## Results

The notebook provides insights into the relationships between the insurance claim amount and various features, as well as the performance of the linear regression model. The VIF analysis helps to ensure that the model is not affected by multicollinearity, leading to more reliable predictions.
