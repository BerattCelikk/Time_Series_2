# Time Series Analysis Project

This project demonstrates various techniques for analyzing time series data, including data loading, exploration, feature engineering, resampling, interpolation, and moving average smoothing. The project is applied to several datasets, such as birth rates, temperature records, and sales data, to uncover patterns, trends, and insights.

## Project Overview

In this project, we perform time series analysis using Python libraries such as `pandas` and `matplotlib`. The key steps of the project include:

1. **Loading and Exploring Time Series Data**  
   The `daily-total-female-births.csv` dataset is used to explore birth rates over time.

2. **Date-Time Features and Window-Based Features**  
   Using the `daily-minimum-temperatures.csv` dataset, we create date-time features (year, month, day) and calculate window-based features like rolling means.

3. **Resampling and Interpolation**  
   The `shampoo-sales.csv` dataset is resampled to different time frequencies (daily, monthly), and missing values are interpolated to fill the gaps.

4. **Moving Average Smoothing**  
   We apply centered and trailing moving averages to the birth data to analyze trends and patterns.

---

## Datasets

### 1. `daily-total-female-births.csv`
- This dataset contains daily total female birth records over several years.
- We explore and visualize birth trends over time.

### 2. `daily-minimum-temperatures.csv`
- This dataset contains daily minimum temperatures for Melbourne, Australia.
- We create date-related features and window-based features (like rolling means).

### 3. `shampoo-sales.csv`
- This dataset contains monthly sales data for shampoo products.
- We resample the data to daily and monthly frequencies and fill missing data through interpolation.

---

## Key Features and Techniques Used

### **Loading and Exploring Time Series Data**
- We load the datasets using `pandas.read_csv()` and convert the date columns to `datetime` format for easy manipulation.

### **Date-Time Features**
- New features like `Year`, `Month`, and `Day` are extracted from the `Date` column to help identify trends and seasonality.

### **Lag Features**
- Lag features are created to examine the impact of previous values (such as the temperature from the previous day) on the current value.

### **Window-Based Features**
- Rolling statistics (e.g., a 3-day moving average) are used to smooth the data and better visualize longer-term trends.

### **Resampling and Interpolation**
- The `shampoo-sales.csv` data is resampled to different time frequencies (daily and monthly).
- Linear interpolation is applied to fill in missing data after resampling, ensuring continuous and accurate time series data.

### **Moving Average Smoothing**
- Both centered and trailing moving averages (with a 7-day window) are applied to birth data to identify underlying trends and reduce noise.

---

## How to Run

1. Clone the repository:
    ```bash
    git clone <your-repository-url>
    ```

2. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the analysis script:
    ```bash
    python time_series_analysis.py
    ```

---

## Example Outputs

### 1. **Birth Rate Trends**  
   Visualization of trends in the daily total female births using line charts.

### 2. **Temperature Analysis**  
   Visualizing temperature patterns and rolling means (moving averages) to observe long-term trends.

### 3. **Shampoo Sales Resampling**  
   Monthly and daily resampling of shampoo sales data and interpolated results.

---

## Tools and Libraries

- `pandas`: For data manipulation and time series analysis.
- `matplotlib`: For data visualization.
- `numpy`: For numerical operations.
- `seaborn`: For advanced data visualization.

---

## Contributing

Feel free to fork this repository, make improvements, or open issues to suggest new features or report bugs.

---

