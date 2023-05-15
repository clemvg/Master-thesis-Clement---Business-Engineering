# Master-thesis-Clement
Master thesis Clément 2023 KU Leuven


**Abstract**: 
Investors typically aim to maximise their returns when they buy or sell stocks in the market. However, predicting stock prices is challenging due to the market's nonlinear and dynamic nature, influenced by a multitude of factors. In order to tackle this issue, this study proposes a one day ahead state-of-the-art hybrid stock price prediction model. The model combines empirical mode decomposition (EMD) with a long-short-term memory (LSTM) model and incorporates news sentiment analysis labeled through FinBERT. The primary goal is to investigate the predictive power of news sentiment on stock prices. The experimental study applies the proposed model to the next day price prediction of the Nasdaq100 index, and the results show that both news sentiment and especially EMD can enhance stock price prediction. In particular, stacking intrinsic mode functions (IMFs), obtained by EMD, in a single LSTM model achieved on average better prediction performance. The main contributions of this research are threefold: first, the thesis proposes a ticker-weighted method to enhance the price-news sentiment correlation; second, we compare two set-ups on how to best use EMD; and finally, we present a nuanced interpretation and common pitfalls of such stock price prediction models.

Specifically, we compared three different model setups: one without EMD, one with EMD applied over multiple LSTMs, and one with EMD stacked - respectively s**et-up 1, 2, and 3 notebooks**.

For addtional questions please contact me through following email address: clement.vangoethem@student.kuleuven.be
