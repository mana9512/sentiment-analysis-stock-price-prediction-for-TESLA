# Tesla Stock Price Prediction using Sentiment Analysis

## Project Overview

This project analyzes the relationship between sentiment in news articles and Tesla (TSLA) stock prices. It implements various time series models to predict stock prices and compares their performance.

## Data

- Stock price data: Historical TSLA stock prices from October 2, 2023 to December 29, 2023, sourced from Yahoo Finance.
- Sentiment data: Sentiment scores derived from published articles about Tesla.

## Methodology

1. Data Preparation:
   - Loaded and preprocessed stock price and sentiment data.
   - Merged daily stock prices with aggregated sentiment scores.

2. Exploratory Data Analysis:
   - Visualized stock price trends and sentiment score distribution.
   - Calculated correlation between sentiment scores and stock prices.

3. Stock Price Prediction Models:
   - Autoregressive (AR) Model
   - Linear Regression
   - Percentage Change Prediction
   - ARIMA Model
   - Direction Prediction (Logistic Regression)

4. Model Evaluation:
   - Used Mean Squared Error (MSE) and Mean Absolute Error (MAE) for performance comparison.

## Key Findings

- ARIMA model outperformed other approaches in predicting Tesla stock prices.
  - ARIMA Performance: MSE: 67.64, MAE: 7.19
- Weak positive correlation (0.22) found between sentiment scores and stock prices.
- Sentiment analysis alone showed limited predictive power for stock price movements (55% accuracy in direction prediction).

## Files in the Repository

- `Final_SentimentAnalysis_vs_TSLAprices.ipynb`: Jupyter notebook containing the full analysis.
- `filtered_prices_and_sentiments.csv`: Dataset with stock prices and sentiment scores.
- `README.md`: This file, providing an overview of the project.

## Requirements

- Python 3.x
- Libraries: pandas, numpy, matplotlib, seaborn, sklearn, statsmodels

## Usage

1. Clone the repository.
2. Install required libraries: `pip install pandas numpy matplotlib seaborn scikit-learn statsmodels`
3. Open and run the Jupyter notebook `SentimentAnalysis_vs_TSLAprices.ipynb`.

## Future Work

- Explore more advanced machine learning models (e.g., LSTM, ensemble methods).
- Incorporate additional external factors and extend the analysis period.
- Investigate the lag between sentiment changes and stock price movements.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
