# Airbnb New York Analysis

## Project Overview
This project aims to analyze Airbnb listings in New York using data science techniques, focusing on insights related to pricing, availability, and trends across different neighborhoods. The analysis covers data collection, preprocessing, exploratory data analysis (EDA), and visualization.

## Data Source
- **Dataset:** Airbnb New York City listings
- **Format:** CSV
- **Key Columns:**
  - `id` - Unique identifier for the listing
  - `name` - Name of the listing
  - `neighbourhood_group` - Broad area classification (e.g., Manhattan, Brooklyn)
  - `neighbourhood` - Specific neighborhood of the listing
  - `room_type` - Type of accommodation (Entire home, Private room, Shared room)
  - `price` - Price per night
  - `minimum_nights` - Minimum nights required to book
  - `number_of_reviews` - Total number of reviews received
  - `last_review` - Date of the most recent review
  - `reviews_per_month` - Average number of reviews per month
  - `calculated_host_listings_count` - Number of listings owned by the host
  - `availability_365` - Number of available days in a year

## Steps in Analysis
### 1. Data Collection
- Download the dataset
- Load it using Pandas

### 2. Data Preprocessing
- Handle missing values - With constants
- Convert data types if necessary - Objects and numerical
- Remove duplicates - If applicable
- Feature engineering (e.g., deriving price per room type, availability rate) - Can implement VIF,RFE,IV

### 3. Exploratory Data Analysis (EDA)
- Generate summary statistics (for both Object and numerical)
- Analyze distributions of key variables
- Identify and visualize outliers
- Perform correlation analysis to detect relationships
- Outlier detection - IQR

### 4. Data Visualization
- **Room Type Distribution:** Normal calculation and used pointplots & distplots
- **Price Trends:** Boxplots or histograms illustrating price variations by neighborhood
- **Availability Heatmaps:** Visualizing availability trends across different areas - (Great inferences)
- **Correlation Heatmaps:** Displaying relationships between price, reviews, and availability

## Tools & Libraries Used
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Plotly

## Next Steps
Beyond visualization, potential next steps include:
- Feature selection and engineering for predictive modeling
- Building machine learning models to forecast prices
- Identifying factors influencing listing popularity
- Business insights for Airbnb hosts and investors

---

## Author
Pranav Giri
