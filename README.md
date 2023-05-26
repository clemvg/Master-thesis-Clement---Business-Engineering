# Master-thesis-Clement
Master thesis Clément 2023 KU Leuven


**Abstract**: 
Investors typically aim to maximise their returns when they buy or sell stocks in the market. However, predicting stock prices is challenging due to the market's nonlinear and dynamic nature, influenced by a multitude of factors. In order to tackle this issue, this study proposes a one day ahead state-of-the-art hybrid stock price prediction model. The model combines empirical mode decomposition (EMD) with a long-short-term memory (LSTM) model and incorporates news sentiment analysis labeled through FinBERT. The primary goal is to investigate the predictive power of news sentiment on stock prices. The experimental study applies the proposed model to the next day price prediction of the Nasdaq100 index, and the results show that both news sentiment and especially EMD can enhance stock price prediction. In particular, stacking intrinsic mode functions (IMFs), obtained by EMD, in a single LSTM model achieved on average better prediction performance. The main contributions of this research are threefold: first, the thesis proposes a ticker-weighted method to enhance the price-news sentiment correlation; second, we compare two set-ups on how to best use EMD; and finally, we present a nuanced interpretation and common pitfalls of such stock price prediction models.

This repository contains the followings files:

CSV and numpy files:
- news__df.7z: news database after preprocessing and filtering out time period and tickers (use 7z software to unzip it)
- sentimentheadlines_postFinBERT: sentiment score (positive, negative, neutral) of news database headlines obtained with FinBERT
- sentimentbodies_postFinBERT.7z: sentiment score (pos, neg, neu) of news database bodies obtained with FinBERT (use 7z software to unzip it)
- Ticker proportions and correlations results: market cap proportion + price-news correlations results
- price.csv: YH Nasdaq100 index ope, close, volumne data
- price.npy: adj close price Nadaq100 numpy array (target variable)
- sentiment_data.npy: best sentiment sentiment time series (input data)

Notebooks:
- News_database_preprocessing: news database preprocessing (from 221k to 42k articles)
- FinBERT and corr_analysis: code to extract sentiment from news database using FinBERT and converting polarity scores to one single score + correlation analysis
- YH_market_cap_prop_retrieval: market cap proportion computations scraped from YH during analyzed time period

The results from the 288 tested model configurations are on the main page alongside the proposed set-up 3(IMFs stacked in one single LSTM model)

For addtional questions please contact me through following email address: clement.vangoethem@student.kuleuven.be
