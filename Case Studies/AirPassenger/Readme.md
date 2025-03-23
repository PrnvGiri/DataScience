# AirPassenger Time Series Analysis

## Project Overview
This project focuses on analyzing the AirPassenger dataset, a time series dataset containing monthly totals of international airline passengers from 1949 to 1960. The primary objectives include checking stationarity, transforming data to achieve stationarity, and applying ARIMA and SARIMAX models for accurate forecasting.

## Data Source
- **Dataset:** AirPassenger dataset
- **Format:** CSV
- **Key Columns:**
  - `Month` - Timestamp (monthly data from 1949 to 1960)
  - `Passengers` - Number of airline passengers per month

## Steps in Analysis

### 1. Checking Stationarity
- Used **Augmented Dickey-Fuller (ADF) test** to check if the time series is stationary.
- Plotted rolling statistics (mean and standard deviation) to visualize stationarity.

### 2. Making Data Stationary
To remove trends and seasonality, the following transformations were applied:
- **Log Transformation:** Reduces variance in the data.
- **Rolling Mean Subtraction:** Removes trend by subtracting the rolling mean.
- **Differencing (Shift Method):** Helps eliminate trends and make the series stationary.

### 3. Time Series Modeling
- **ARIMA (AutoRegressive Integrated Moving Average):**
  - Applied to model the trend and forecast future values.
  - Selected optimal p, d, q parameters based on ACF and PACF plots.
- **SARIMAX (Seasonal AutoRegressive Integrated Moving Average with eXogenous factors):**
  - Used to handle seasonality effectively.
  - Seasonal parameters (P, D, Q, S) were determined using seasonal decomposition.
  - In our case we will be having 12 as our window size

### 4. Forecasting
- Compared ARIMA and SARIMAX model predictions.
- Evaluated models using metrics like AIC, RMSE, and MAPE.
- Visualized actual vs. predicted passenger counts over time.

## Tools & Libraries Used
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, pmdarima, itertools

## Next Steps
Future improvements may include:
- Experimenting with Prophet for forecasting. - (FB Prophet)
- Handling external factors affecting air traffic.
- Deploying the model for real-time predictions. - Via Cloud platforms

---

## Author
**Pranav Giri**
