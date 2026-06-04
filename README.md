# Stock Price Time Series Analysis

## Problem Statement

The objective of this project is to perform Time Series Analysis on historical stock price data to identify patterns, trends, and seasonal behavior in stock market performance. The analysis aims to provide meaningful insights into stock price movements over time and forecast future values using statistical time series techniques.

Key objectives include:

- Analyze long-term stock price trends.
- Detect seasonal patterns and recurring behaviors.
- Measure stock return volatility.
- Examine trading turnover behavior.
- Forecast future stock prices.
- Generate actionable insights from historical market data.

---

## Dataset Details

### Dataset Name
Stock Price Dataset

### Dataset Size
- Total Records: 1,498
- Total Features: 9

### Features Description

| Feature | Description |
|----------|------------|
| mic | Market Identifier Code |
| symbol | Stock Symbol |
| isin | International Securities Identification Number |
| date | Trading Date |
| open_value | Opening Stock Price |
| high_value | Highest Stock Price of the Day |
| low_value | Lowest Stock Price of the Day |
| last_value | Closing/Last Traded Stock Price |
| change_prev_close_percentage | Percentage Change from Previous Closing Price |
| turnover | Trading Turnover Volume |

### Data Preprocessing

The following preprocessing steps were performed:

- Converted the `date` column into datetime format.
- Sorted records chronologically.
- Set the date column as the index for time series analysis.
- Handled missing values using linear interpolation.
- Generated additional features such as:
  - Daily Returns
  - 30-Day Moving Average
  - 90-Day Moving Average
  - Rolling Volatility

---

## Approach

### 1. Data Loading and Exploration

- Loaded the stock price dataset using Pandas.
- Examined dataset structure and summary statistics.
- Checked for missing values and data quality issues.

### 2. Trend Analysis

- Visualized stock closing prices over time.
- Identified overall upward and downward movements.
- Analyzed long-term market behavior.

### 3. Moving Average Analysis

- Calculated:
  - 30-Day Moving Average
  - 90-Day Moving Average

- Compared short-term and long-term trends.
- Evaluated bullish and bearish market conditions.

### 4. Daily Return Analysis

- Computed percentage daily returns.
- Examined stock performance consistency.
- Measured day-to-day fluctuations.

### 5. Volatility Analysis

- Calculated rolling 30-day volatility.
- Assessed risk levels associated with stock movements.
- Identified periods of high and low market uncertainty.

### 6. Seasonality Detection

- Performed monthly trend analysis.
- Applied seasonal decomposition to separate:
  - Trend Component
  - Seasonal Component
  - Residual Component

- Investigated recurring market patterns.

### 7. Turnover Analysis

- Analyzed turnover trends over time.
- Studied market activity and trading intensity.

### 8. Correlation Analysis

- Generated a correlation heatmap among stock variables.
- Identified relationships between:
  - Opening Price
  - Closing Price
  - High Price
  - Low Price
  - Turnover

### 9. Forecasting

- Implemented Exponential Smoothing.
- Forecasted future stock prices for the next 30 periods.
- Visualized historical and predicted stock prices.

---

## Results

### Key Findings

- Historical stock prices exhibited noticeable time-based fluctuations.
- Moving average analysis successfully highlighted long-term trends.
- Daily return analysis revealed periods of positive and negative performance.
- Volatility analysis identified varying levels of market risk across the trading period.
- Seasonal decomposition detected underlying trend and seasonal components within the stock price series.
- Trading turnover showed changing levels of market participation over time.
- Strong correlations were observed among price-related variables.
- The forecasting model generated future stock price estimates based on historical patterns.

### Generated Visualizations

The project produced the following visual outputs:

1. Stock Price Trend Analysis
2. Moving Average Analysis
3. Daily Returns Trend
4. Rolling Volatility Analysis
5. Monthly Trend Analysis
6. Monthly Seasonality Analysis
7. Seasonal Decomposition Plot
8. Daily Return Distribution
9. Turnover Trend Analysis
10. Correlation Heatmap
11. Future Stock Price Forecast

### Output Files

- `01_Stock_Price_Trend.png`
- `02_Moving_Average_Analysis.png`
- `03_Daily_Returns.png`
- `04_Volatility_Analysis.png`
- `05_Monthly_Trend.png`
- `06_Monthly_Seasonality.png`
- `07_Seasonal_Decomposition.png`
- `08_Return_Distribution.png`
- `09_Turnover_Trend.png`
- `10_Correlation_Heatmap.png`
- `11_Stock_Forecast.png`
- `Forecast_30_Days.csv`
- `Time_Series_Insights.txt`
