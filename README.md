# Apple-Stock-Analysis

## About the Dataset
The data used in this project consists of the historical stock prices of Apple obtained via Yahoo Finance. The dataset contains the following variables:

* **Date (May 2014 - May 2020)**
* **Open**
* **High**
* **Low**
* **Close**
* **Adjusted Close**
* **Volume**


## Project Description
This project analyzes the historical stock prices of Apple and generates buy and sell signals based on the Simple Moving Average (SMA) crossover strategy. The strategy involves using two SMAs: a short-term SMA (30 days) and a long-term SMA (100 days).

## Files

**Apple Stock Analysis.ipynb**: The Jupyter Notebook containing the entire analysis, including data preprocessing, calculation of SMAs, generation of buy/sell signals, and visualization.

**stock.csv**: The dataset containing historical stock prices of Apple.


## Analysis
The analysis involves the following steps:

1. **Data Loading and Preprocessing**:

* The dataset is loaded and the relevant columns are selected.
* The "Adj Close Price" column is renamed to "Apple".

2. **Calculation of Simple Moving Averages (SMA)**:

* The short-term SMA (SMA30) is calculated using a rolling window of 30 days.
* The long-term SMA (SMA100) is calculated using a rolling window of 100 days.

3. **Generation of Buy and Sell Signals**:

* Buy signals are generated when SMA30 crosses above SMA100.
* Sell signals are generated when SMA30 crosses below SMA100.
* Hold signals are generated when SMA30 equals SMA100.


## Visualization:

* The historical adjusted closing prices of Apple stock are plotted along with SMA30 and SMA100.
* Buy and sell signals are marked on the plot using green upward-pointing triangles (^) and red downward-pointing triangles (v) respectively.

## Conclusion
This visualization provides a comprehensive view of Apple's stock performance, with clear indicators for buy and sell signals based on the SMA crossover strategy. It allows investors or analysts to assess the strategy's effectiveness and make informed decisions based on historical data.


## Additional Information
* The buy and sell signals are generated using a simple SMA crossover strategy, which may not account for all market conditions and may require further optimization and validation before being used in real trading scenarios.

* The project demonstrates a basic example of technical analysis and can be extended with additional indicators and strategies.
