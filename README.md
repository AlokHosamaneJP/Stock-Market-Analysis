# Stack_Market_Analysis-GOOGLE

## Overview
This project analyzes historical stock market data for major tech companies such as Apple (AAPL), Google (GOOG), Microsoft (MSFT), and Amazon (AMZN). By leveraging Python's data analysis and machine learning libraries, it demonstrates the process of data retrieval, exploratory data analysis (EDA), and building predictive models (e.g., LSTM for time-series forecasting).

## Features
  - Data Retrieval: Automatically fetches historical stock prices using yFinance.
  - Exploratory Data Analysis (EDA): Analyzes stock trends, volatility, and statistics using Pandas, Matplotlib, and Seaborn.
  - Visualization: Generates insightful charts, such as stock price trends, moving averages, and correlation heatmaps.
  - LSTM Model: Implements a Long Short-Term Memory (LSTM) neural network to predict future stock prices.
## Model Explanation
  1. ### Long Short-Term Memory (LSTM)
     The LSTM model is designed for time-series forecasting, making it ideal for predicting stock prices. Here's how it works:
      - Input Shape: The model takes in a sequence of stock prices over 60 days (timesteps) to predict the next price.
      - Architecture:
          - Two stacked LSTM layers to capture long-term dependencies in the stock price data.
          - Two dense layers for regression to predict the final price.
      - Loss Function: Mean Squared Error (MSE), which minimizes the squared differences between actual and predicted prices.
      - Optimizer: Adam, a gradient-based optimization algorithm.

## Visualizations
The project includes multiple visualizations to better understand stock trends and relationships. Here are the key plots:

  1. Daily Return Distributions
      Description: Displays histograms of daily returns for tech stocks like Apple, Google, Microsoft, and Amazon.
      Purpose:
      - Highlights the distribution of percentage changes in daily stock prices.
      - Helps identify the average daily return and the volatility of each stock.
      ![dailyreturn](https://github.com/user-attachments/assets/2c9608fa-c9c7-4117-a921-6231f0eef25e)

  2. Closing Prices Over Time 
      Description: Line plots showing the closing prices of stocks over time for Apple, Google, Microsoft, and Amazon.
      Purpose:
      - Visualizes trends in stock performance.
      - Identifies key periods of growth or decline for each stock.
      ![closing](https://github.com/user-attachments/assets/d872ccc6-a9ad-4902-bc52-4609d5a42e91)

  3. Moving Averages 
      Description: Plots the actual stock prices along with 10-day, 20-day, and 50-day moving averages for each stock.
      Purpose:
      - Identifies long-term trends by smoothing out short-term price fluctuations.
      - Useful for detecting bullish or bearish signals.
     ![ma](https://github.com/user-attachments/assets/20625aee-e9b4-402a-9de3-db60df03dd83)

  4. Percentage Changes
      Description: Scatter plots showing daily percentage changes for each stock.
      Purpose:
      - Examines day-to-day fluctuations in stock prices.
      - Helps assess the level of volatility for different stocks.
     ![Percentage change](https://github.com/user-attachments/assets/1ceef9af-5a0c-46dd-8074-fbcfb4d74465)

  5. Risk vs. Return
      Description: Scatter plot showing the risk (volatility) vs. expected return for tech stocks.
      Purpose:
      - nalyzes the trade-off between risk and return.
      - For example, higher-risk stocks like Google or Amazon may offer higher returns, while lower-risk stocks like Microsoft provide stability.
      ![returnvs risk](https://github.com/user-attachments/assets/70b235f0-306a-4eb2-90d3-0d93449b4460)

  6. Sales Volume
      Description: Line plots showing daily trading volume for each stock.
      Purpose:
      - Identifies periods of high or low trading activity.
      - Helps detect significant market events (e.g., earnings reports or news announcements) that increase trading volume.
      ![sales_volume](https://github.com/user-attachments/assets/8cc6048a-c87f-4786-9ad2-e486cf622a4b)

  7. Correlation Heatmap
      Description: A heatmap showing correlations between the daily closing prices of different tech stocks.
      Purpose:
      - Highlights relationships between stocks.
      - For example, a strong correlation (close to 1) indicates that two stocks move together, while a low or negative correlation indicates independent or opposite movements. We can understand that all the companies have positive correlation.
      ![Corr](https://github.com/user-attachments/assets/a5311a66-294d-48fe-bcb1-c7c57d92e544)
      ![corr2](https://github.com/user-attachments/assets/3984aaea-b223-4640-bcc4-762038316156)

  8. Model Predictions (Pred.png)
      Description: Line plot comparing actual stock prices (training and validation data) with the model's  predictions.
      Purpose:
      - Evaluates how well the LSTM model predicts future stock prices.
      - Shows the effectiveness of the model in capturing historical trends.
     ![Pred](https://github.com/user-attachments/assets/f442c6e8-b1cc-4232-8e0b-524c331eb6d6)


## Results
  Exploratory Analysis:
      Stock prices for AAPL, GOOG, MSFT, and AMZN exhibit distinct patterns, with periodic increases and drops.
      Correlations among the companies suggest strong co-movement, especially between GOOG and MSFT.
   LSTM Model Predictions:
      - The LSTM model provides reasonably accurate predictions for the next day's stock prices.
      - Performance is evaluated using metrics like MSE (Mean Squared Error).
