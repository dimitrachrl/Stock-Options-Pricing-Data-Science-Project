# Stock-Options-Pricing-Data-Science-Project
This repository contains the Stock Options Pricing Project, which was undertaken as part of the DSO 530 course.

## Business Problem

The primary objective of this project is to optimize the valuation and pricing of stock options. Stock options play a crucial role in financial markets, allowing investors to make decisions based on their risk tolerance and market conditions. In this project, we aim to address the following key aspects:

1. **Optimizing Option Valuation**: We seek to optimize the valuation of options, considering factors such as current option value, current asset value, option strike price, interest rate, and time to maturity. This optimization will enable more accurate pricing and valuation, contributing to well-informed investment decisions.

2. **Identifying the Best Purchase Period**: Determining the optimal time to purchase an asset at a given price is essential for investors. By analyzing historical data and market conditions, we aim to identify the best periods for asset acquisition. This knowledge empowers investors to make strategic decisions.

3. **Utilizing the Black-Scholes Model**: The Black-Scholes model is a renowned mathematical framework for estimating the value of financial options. We leverage this model to provide accurate estimations of option values as a foundation for our analysis.

4. **Machine Learning-Based Approach**: In addition to the Black-Scholes model, we explore the application of machine learning (ML) techniques to determine option values. ML models offer the advantage of capturing complex patterns and relationships within the data, potentially enhancing the accuracy of option pricing.

## Data Source
Datasets provided: option_train.csv and option_test_wolabel.csv
The training data set has information on 1,680 separate options. 
In particular, for each option we have recorded
• Value (C): Current option value
• S: Current asset value
• K: Strike price of option
• r: Annual interest rate
• tau: Time to maturity (in years)
• BS: The Black-Scholes formula was applied to this data (using some 𝜎) to get C_pred.
and If an option has C_pred – C > 0, i.e., the prediction over estimated the option value, we associate that option by (Over); otherwise, we associate that option with (Under).

## Objective
The core idea of the project is to use the training data to build statistical/ML models with
1) Value as the response (i.e., a regression problem) and then
2) BS as the response (i.e., a classification problem).
Ultimately you will select what you consider to be the most accurate approach and use it to make predictions for C and BS on the 1,120 options in the test data set. You will submit these two sets of predictions. I will compare these predictions in comparison to the actual Value and BS results on the test options (which I have), in terms of out-of-sample R squared and classification error, respectively.
