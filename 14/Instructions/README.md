# LSTM Stock Predictor

![deep-learning.jpg](Images/deep-learning.jpg)

Due to the volatility of cryptocurrency speculation, investors will often try to incorporate sentiment from social media and news articles to help guide their trading strategies. One such indicator is the [Crypto Fear and Greed Index (FNG)](https://alternative.me/crypto/fear-and-greed-index/) which attempts to use a variety of data sources to produce a daily FNG value for cryptocurrency. 

This assignment task was mentioned to help build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.

Deep learning recurrent neural networks was implemented to model bitcoin closing prices. One model had used the FNG indicators to predict the closing price while the second model had used a window of closing prices to predict the nth closing price.

The below tasks are done:

1. [Prepared the data for training and testing](#prepare-the-data-for-training-and-testing)
2. [Built and trained custom LSTM RNNs](#build-and-train-custom-lstm-rnns)
3. [Evaluated the performance of each model](#evaluate-the-performance-of-each-model)

- - -

### Files

[Closing Prices Starter Notebook](Starter_Code/lstm_stock_predictor_closing.ipynb)

[FNG Starter Notebook](Starter_Code/lstm_stock_predictor_fng.ipynb)


### Prepared the data for training and testing

For the Fear and Greed model, the FNG values were used to try and predict the closing price. 

For the closing price model, previous closing prices were used to try and predict the next closing price. 

Each model used 70% of the data for training and 30% of the data for testing.

Applied a MinMaxScaler to the X and y values to scale the data for the model.

Finally, reshaped the X_train and X_test values to fit the model's requirement of samples, time steps, and features. 

### Built and trained custom LSTM RNNs

In each Jupyter Notebook, created the same custom LSTM RNN architecture. In one notebook, fitted the data using the FNG values. In the second notebook, fitted the data using only closing prices.

Used the same parameters and training steps for each model.

### Evaluate the performance of each model

Finally, used the testing data to evaluate each model and compare the performance.

From the above answered the following:

> Which model has a lower loss?

> Which model tracks the actual values better over time?

> Which window size works best for the model?
To determine the model that works best, the window size was altered and the data inferred was saved in [Analysis.csv](Starter_Code/Analysis.csv) which is located in the same folder as the python files.
- - -

### Resources

[Keras Sequential Model Guide](https://keras.io/getting-started/sequential-model-guide/)

[Illustrated Guide to LSTMs](https://towardsdatascience.com/illustrated-guide-to-lstms-and-gru-s-a-step-by-step-explanation-44e9eb85bf21)

[Stanford's RNN Cheatsheet](https://stanford.edu/~shervine/teaching/cs-230/cheatsheet-recurrent-neural-networks)