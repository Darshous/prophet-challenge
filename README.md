
# MercadoLibre Search Traffic Analysis

## Project Overview

This project analyzes the search traffic patterns for **MercadoLibre**, the most popular e-commerce platform in Latin America. The objective is to use **Prophet**, a forecasting tool, to find patterns and trends in the search traffic data and make predictions. The key focus areas of the analysis include:

1. **Identifying unusual patterns** in hourly search traffic during key corporate events, such as financial reports.
2. **Mining the search traffic data for seasonality** to uncover daily and weekly patterns of interest.
3. **Correlating search traffic with stock price patterns**, investigating whether there is any predictable relationship.
4. **Building a time series model using Prophet** to forecast future search traffic and analyze its components.

## Dataset

The dataset consists of hourly search traffic data for MercadoLibre, along with forecasted values. The `Prophet` forecasting model is applied to identify trends and predict future search traffic levels.

## Key Steps

### 1. Unusual Patterns in Hourly Google Search Traffic
- Filtered the data to analyze the month of May 2020, when MercadoLibre released its quarterly financial results.
- Identified any unusual spikes in search traffic and compared the total search traffic with the monthly median.

### 2. Seasonality Analysis
- Grouped the hourly data by day and week to uncover patterns of search traffic.
- Analyzed which hours of the day and which days of the week showed the most interest in MercadoLibre.

### 3. Correlation with Stock Price
- Merged search traffic data with stock price data.
- Investigated if there is any correlation between search traffic (lagged by 1 hour) and stock price volatility or returns.

### 4. Time Series Forecasting with Prophet
- Built a forecasting model using `Prophet` to predict future search traffic trends.
- Visualized the forecast along with confidence intervals and analyzed daily and weekly seasonality.
- Identified the lowest points of search interest within the year 2020.

## Results

- **May 2020 Search Traffic:** A spike in search traffic was observed around the time of the financial results.
- **Seasonality:** The analysis uncovered daily and weekly patterns, with specific times showing increased interest in MercadoLibre.
- **Correlation with Stock Price:** No strong correlation was found between lagged search traffic and stock price volatility.
- **Time Series Forecasting:** The model provided insights into future traffic, including periods of lower and higher interest.

## Tools and Libraries

- **Pandas**: For data manipulation and analysis.
- **Prophet**: For building the forecasting model.
- **Matplotlib**: For visualizing the results.

## Instructions for Running the Code

1. Clone this repository.
2. Install the necessary dependencies using `pip install -r requirements.txt`.
3. Run the Jupyter notebook to replicate the analysis and visualize the results.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
