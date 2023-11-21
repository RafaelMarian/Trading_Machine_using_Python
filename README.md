Unsupervised Learning Trading Strategy
Overview

This project focuses on developing an unsupervised learning-based trading strategy by leveraging various machine learning techniques. The strategy involves the following key steps:

    Data Collection:
        Download or load historical stock prices data for the S&P 500 index.

    Feature and Indicator Calculation:
        Calculate different features and indicators for each stock in the dataset. These could include metrics like moving averages, relative strength index (RSI), and other relevant technical indicators.

    Data Aggregation and Filtering:
        Aggregate the calculated features on a monthly basis and filter the top 150 most liquid stocks. This step aims to focus on a subset of stocks for further analysis.

    Return Calculation:
        Calculate monthly returns for different time horizons for the selected stocks.

    Fama-French Factor Analysis:
        Download Fama-French factors and calculate rolling factor betas for the selected stocks. This analysis helps to understand the exposure of the stocks to various market factors.

    K-Means Clustering:
        For each month, fit a K-Means clustering algorithm to group similar assets based on their calculated features. This step aims to identify clusters of stocks with similar behavior.

    Portfolio Formation:
        For each month, select assets based on the clusters obtained from the K-Means algorithm. Form a portfolio using an Efficient Frontier approach with maximum Sharpe ratio optimization. This helps in constructing a well-balanced portfolio with optimal risk-return characteristics.

    Performance Visualization:
        Visualize the portfolio returns over time and compare them to the benchmark returns, such as the S&P 500 index. This step provides insights into the effectiveness of the developed trading strategy.

Dependencies

    Python 3.x
    Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, yfinance (for downloading financial data), and any additional libraries used in the project.
