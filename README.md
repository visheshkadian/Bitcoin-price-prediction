# Bitcoin-price-prediction

Abstract:<br />
This document deal ever changing price of bitcoins or in general cryptocurrency. The fluctuations in the price of these cryptocurrency can be many things like personal, no authorized sanctions, disbelief time to time. This can be seen in recent years when practically non existing cryptocurrency like dogecoin by some comment from Elon Musk sore higher prices. This makes you think that this cryptocurrency is more like gambling other calculated change in price like in case different classic money. For that purpose, we tried to predict bitcoin prices by creating different models using different regression techniques.
This doesn’t mean that the model we have created in document perfect for future prices also these models created using previous 5 years bitcoin price data by dividing between training and testing data. Score or accuracy we talk about in this document is just about overlapping real prices with predicted prices given models.

Keywords: models, data, regression, price, predict, bitcoin<br /><br />
Introduction:<br />
Virtual currencies are a form of cryptocurrency which is an impressive technical achievement in digital marketing, nevertheless. Virtual currencies live on, and they couldn’t fully replace fiat or conventional currencies. The popularity of virtual currencies is due to its innovative characteristics such as transparency, simplicity, and increasing acceptance through the world. In the current time, bitcoin is the popular flourishing virtual currency. Bitcoin may be a peer-to-peer cryptocurrency during which all transactions aren't regulated or controlled by any third party. Third-party intervention between customers is impossible. It is highly volatile market price working 24/7. Market capitalization of bitcoin is increased through time to time. In the current time, more than 71 billion of dollars publicly traded. Due to its open-source nature, clear, transparent, simple, and time is saving which leads all virtual currencies within the world. In this project we will try to predict prices of bitcoin using graphs and various model for analysis.
Literature Survey:<br />
Our project builds on various previous research. The purpose of one of study is to predict the price of Bitcoin and changes therein using models.
These are the different models we implemented in our project by the use of machine learning
Linear Regression<br />
Lasso Regression<br />
Ridge Regression<br />
KNN Regression<br />
Polynomial Regression<br />
SVM regression<br />
By using these models we made comparison between them by accuracy<br /><br />
Problem Definition:<br />
We present a Bitcoin price fluctuation prediction problem since many investors care more about whether the sudden rise or fall is worth following. This problem can be simply described as the different behaviors of the Bitcoin price after a certain percentage change (i.e., rise or fall). For instance, if the Bitcoin price reverses after a rapid rising, following the rising price is harmful to investors since investors would make a loss in this case. Otherwise, if the price keeps rising after a rapid rising, it is good for investors since they can make more profits when following the rapid rising. We try to use all methods and models for prediction of prices of Bitcoin. Then use that predicted data prices for better and more accurate result of prices of bitcoin.

Methodology:<br />

Dataset Description:<br />
We have got the bitcoin price data from Yahoo Finance. In this data contain columns Date, Open, High, Low, Close, Adj Close. We are only using column Date and Adj Close. After we divide the data between training data and test data both data will split into Y_train, X_train or Y_test, X_test respectively. In case of training data both of dataset will be use to create model. In case of test data, one dataset will be used to predict values and other dataset use check how predicted value overlap over real value.
