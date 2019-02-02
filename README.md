# Real-Estate-Valuation-using-Non-Linear-Regression

This is an update to the previous versions of linear regression. After getting to know other types of regression, I find that the data in this real estate valuation file does not show direct linear relationship with each other. Hence, linear regression cannot be used. Here, I implemented a non-linear regression method as I found that there is one feature that shows a clear non-linear relationship with the label. Let's get into the meat of the project.

Project title: Implementation of Non-Linear Regression on Real Estate Valuation data to predict the house price per unit area

Data source: https://archive.ics.uci.edu/ml/datasets/Real+estate+valuation+data+set

The feature set that I used here is "Distance to the nearest convenience store" while the label is "Price of house per unit area"
These two feature and label shows a non-linear relationship, clearly a logistic function, and is suitable for non-linear regression method.
Plotting the data, and finding the best fit of parameters, I used K-fold Cross Validation to make sure that the score in the end is consistent, so as to provide a good fit. Here the R-2 score may not be the highest (0.40), but the mean absolute error is pretty low at 0.04, while the residual sum of squares, or MSE is 0.00. This clearly shows that using non-linear regression perfectly suits the data chosen.

Data is provided by:
https://archive.ics.uci.edu/ml/datasets/Real+estate+valuation+data+set

Original Owner and Donor 
Name: Prof. I-Cheng Yeh 
Institutions: Department of Civil Engineering, Tamkang University, Taiwan. 
Email: 140910 '@' mail.tku.edu.tw 
TEL: 886-2-26215656 ext. 3181 
Date Donated: Aug. 18, 2018 

Data Set Information:
The market historical data set of real estate valuation are collected from Sindian Dist., New Taipei City, Taiwan. The â€œreal estate valuationâ€ is a regression problem. The data set was randomly split into the training data set (2/3 samples) and the testing data set (1/3 samples).

Attribute Information:
The inputs are as follows 
X1=the transaction date (for example, 2013.250=2013 March, 2013.500=2013 June, etc.)
X2=the house age (unit: year) 
X3=the distance to the nearest MRT station (unit: meter) 
X4=the number of convenience stores in the living circle on foot (integer) 
X5=the geographic coordinate, latitude. (unit: degree) 
X6=the geographic coordinate, longitude. (unit: degree) 

The output is as follow 
Y= house price of unit area (10000 New Taiwan Dollar/Ping, where Ping is a local unit, 1 Ping = 3.3 meter squared) 

Relevant Papers:

Yeh, I. C., & Hsu, T. K. (2018). Building real estate valuation models with comparative approach through case-based reasoning. Applied Soft Computing, 65, 260-271.


Yeh, I. C., & Hsu, T. K. (2018). Building real estate valuation models with comparative approach through case-based reasoning. Applied Soft Computing, 65, 260-271.
