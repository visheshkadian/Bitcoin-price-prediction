# Bitcoin-price-prediction

Abstract:<br />
This project deal ever changing price of bitcoins or in general cryptocurrency. The fluctuations in the price of these cryptocurrency can be many things like personal, no authorized sanctions, disbelief time to time. This can be seen in recent years when practically non existing cryptocurrency like dogecoin by some comment from Elon Musk sore higher prices. This makes you think that this cryptocurrency is more like gambling other calculated change in price like in case different classic money. For that purpose, we tried to predict bitcoin prices by creating different models using different regression techniques.
This doesn’t mean that the model we have created in document perfect for future prices also these models created using previous 5 years bitcoin price data by dividing between training and testing data. Score or accuracy we talk about in this project is just about overlapping real prices with predicted prices given models.

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
Description of Training Data

![image](https://user-images.githubusercontent.com/72352984/130312752-baf29494-92c5-44dc-8035-4585987930e2.png)

Description of Test Data

![image](https://user-images.githubusercontent.com/72352984/130312758-462ec850-5e2a-4cde-a255-84d7b6906dd2.png)

Linear Regression-

It is a way define relationship between two variables. In this regression model target prediction value based on independent variables. For our purpose we try to create a Linear Regression model using training data. 
y = B0 + B1*x
y = value to be predicted
x = independent variable
B0 = intercept or bias coefficient
B1 = scale factor coefficient
When a coefficient becomes zero, it effectively removes the influence of the input variable on the model and thus from the prediction made up of the model (0 * x = 0). This becomes relevant if you check out regularization methods that change the training algorithm to scale back the complexity of regression models by putting pressure on absolutely the size of the coefficients, driving some to zero.

Lasso Regression:

The “LASSO” stands for Least Absolute Shrinkage and Selection Operator. Lasso regression is a regularization technique. It is used over regression methods for a more accurate prediction. This model uses shrinkage. Shrinkage is where data values are shrunk towards a central point as the mean. The lasso procedure encourages simple, sparse models (i.e. models with fewer parameters).
Residual Sum of Squares + λ * (Sum of the absolute value of the magnitude of coefficients)

![image](https://user-images.githubusercontent.com/72352984/130312791-c7843e97-2e28-4ed5-aebd-35c884b49507.png)


Where,
λ denotes the amount of shrinkage.
λ = 0 implies all features are considered and it's like the rectilinear regression where only the residual sum of squares is taken into account to create a predictive model
λ = ∞ implies no feature is considered i.e, as λ closes to infinity it eliminates more and more features
The bias increases with increase in λ
variance increases with decrease in λ

Ridge Regression:

Ridge regression is used to analyze data which have multicollinearity. This method performs L2 regularization. In ridge regression, the primary step is to standardize the variables (both dependent and independent) by subtracting their means and dividing by their standard deviations. This causes a challenge in notation since we must somehow indicate whether the variables in a particular formula are standardized or not. As far as standardization cares, all ridge regression calculations are supported standardized variables.
Y = XB + e
Where Y is that the variable, X represents the independent variables, B is that the regression coefficients to be estimated, and e represents the errors are residuals.

KNN Regression:

K nearest neighbors may be a simple algorithm that stores all available cases and predict the numerical target supported a similarity measure (e.g., distance functions). A simple implementation of KNN regression is to calculate the average of the numerical target of the K nearest neighbors. Another approach uses an inverse distance weighted average of the K nearest neighbors. KNN regression uses the same distance functions as KNN classification.
Choosing the optimal value for K is best done by first inspecting the info. In general, a large K value is more precise as it reduces the overall noise.

![image](https://user-images.githubusercontent.com/72352984/130312811-a6e146d6-d9c3-4bca-ad46-0322b50a5389.png)

Choosing the optimal value for K is best done by first inspecting the data. In general, a large K value is more precise as it reduces the overall noise.

Polynomial Regression:

Polynomial Regression is a regression algorithm that models the relationship between a dependent(y) and independent variable(x) as nth degree polynomial. The Polynomial Regression equation is given below:
                              y= b0+b1x1+ b2x12+ b2x13+...... bnx1n
It is also called the special case of Multiple Linear Regression in ML. Because we add some polynomial terms to the Multiple Linear regression equation to convert it into Polynomial Regression.It is a linear model with some modification in order to increase the accuracy.The dataset used in Polynomial regression for training is of non-linear nature.It makes use of a linear regression model to fit the complicated and non-linear functions and datasets.Hence, "In Polynomial regression, the original features are converted into Polynomial features of required degree (2,3,..,n) and then modeled using a linear model."

SVM regression:

More formally, a support-vector machine constructs a hyperplane or set of hyperplanes in a high- or infinite-dimensional space, which can be used for classification, regression, or other tasks like outliers detection.Intuitively, a good separation is achieved by the hyperplane that has the largest distance to the nearest training-data point of any class (so-called functional margin), since in general the larger the margin, the lower the generalization error of the classifier.

Y = wx+b (equation of hyperplane)
The boundary condition is:
-a < Y- wx+b < +a 


![image](https://user-images.githubusercontent.com/72352984/130312841-27ed42f6-a767-4c6f-8f02-520054f165d0.png)

