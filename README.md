# Advanced Regression Assignment
> The aim of this project is to build a regression model with regularisation to predict the actual prices of house, given the dataset of previous sale of houses in Australia.

## Problem Statement
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.
 
The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

- Which variables are significant in predicting the price of a house?
- How well those variables describe the price of a house?

## Business Goal 
We should build a model to predict the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns.

## Inference

Ridge Model:
- Optimal value of lambda for Ridge regression is 0.4 
- Train and Test R2 values are 0.897 and 0.887

Lasso Model:
- Optimal value of lambda for Lasso regression is 0.0001
- Train and Test R2 values are 0.892 and 0.873

Even though R2 values for Ridge and Lasso models are similar, we are preferring Lasso Model as few of the co-efficients are pushed to zero.

Top 10 variables that are significant in predicting the price of a house obtained from Lasso regression are:

1. GrLivArea(0.307061)
2. OverallQual(0.200335)
3. OverallCond(0.108886)
4. TotalBsmtSF(0.10485)
5. MSZoning_FV(0.084748)
6. GarageCars(0.083943)
7. MSZoning_RL(0.072104)
8. MSZoning_RH(0.063511)
9. KitchenAbvGr(-0.060434)
10. BsmtFullBath(0.05245)

## Libraries Used
- pandas
- numpy
- matplotlib.pyplot
- seaborn
- sklearn

## Acknowledgments - 
- https://towardsdatascience.com/
- https://www.analyticssteps.com/
- https://medium.com/
- https://stackoverflow.com/
- https://www.geeksforgeeks.org/
