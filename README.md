# Black-Friday-Sales-Prediction
  Solution to Analytics Vidhya Black Friday Sales Hackathon Problem

## Problem Statement
A retail company “ABC Private Limited” wants to understand the customer purchase behaviour (specifically, purchase amount) against various products of different categories. They have shared purchase summary of various customers for selected high volume products from last month.
The data set also contains customer demographics (age, gender, marital status, city_type, stay_in_current_city), product details (product_id and product category) and Total purchase_amount from last month.

Now, they want to build a model to predict the purchase amount of customer against various products which will help them to create personalized offer for customers against different products.

Variable | Definition
--- | ---
User_ID | User ID
Product_ID | Product ID
Gender | Sex of User
Age | Age in bins
Occupation | Occupation (Masked)
City_Category | Category of the City (A,B,C)
Stay_In_Current_City_Years | Number of years stay in current city
Marital_Status| Marital Status
Product_Category_1| Product Category (Masked)
Product_Category_2| Product may belongs to other category also (Masked)
Product_Category_3| Product may belongs to other category also (Masked)
Purchase | Purchase Amount (Target Variable)

## Evaluation Metric
The evaluation metric used is **root mean squared error** (RMSE). 

## Approach
The solution to the problem involves predicting the purchase amount for the various products, regressor models have to be used. Out of the three models tested, XGBoost and CatBoost models have identical RMSE of ~2441 and R-squared values of ~0.75 and perform better than LightGBM. Therefore, combination of XGBoost and CatBoost regressors is used to predict the values of purchase amount.   
 

