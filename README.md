# HOUSE PRICE PREDICTION

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.



 ## Table Of Contents:
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)



## General-Information

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:
- Which variables are significant in predicting the price of a house, and
- How well those variables describe the price of a house.

 Also, determine the optimal value of lambda for ridge and lasso regression.

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.



## Technologies-Used:

- Jupyter Notebook(Anaconda 3) - version 6.4.8
- Python3 - version 3.10
- numpy - version 1.21.5
- pandas - version 1.4.2
- matplotlib - version 3.5.1
- seaborn - version 0.11.2
- sklearn
- statsmodels



## Conclusions:

After checking the model using Linear Regression, we get R2 score very low, hence we model Lasso and Ridge Regression.

**Optimal value for both Lasso and Ridge models turned out to be:**
- Optimal value of alpha for Lasso model: 0.0001
- Optimal value of alpha for Ridge model: 20

**The 5 most important variables turned out to be as mentioned below:**

- Lasso model:
1. MSSubClass
2. RoofMatl_WdShngl
3. RoofMatl_CompShg
4. RoofMatl_Roll
5. RoofMatl_Membran

- Ridge model:
1. MSSubClass
2. OverallCond
3. BsmtFullBath
4. Neighborhood_Crawfor
5. Neighborhood_NridgHt

The Mean squared Error in case of Ridge and Lasso are:
- Ridge: 0.019450509001835214
- Lasso: 0.020219075353064733
The Mean squared error of Lasso and Ridge are almost equal. 
Also, since Lasso helps in feature reduction (assigns zero value to insignificant features) Lasso is a better model over Ridge. Therefore the variables predicted by Lasso can be applied for choosing significant variables in predicting the price of the house.



## Acknowledgements:

- This project was inspired by UpGrad Advance Regression Course
- References - google.com, stackoverflow.com



## Contact:

Created by ShreerakshaS - feel free to contact me!
