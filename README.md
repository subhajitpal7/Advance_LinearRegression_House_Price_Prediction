# House Price Prediction (Advanced Regression)
> A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file train.csv.A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file train.csv.


## Table of Contentss
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Model Building and Prediction](#model-building-and-prediction)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularization in order to predict the actual value of the prospective properties and decide whether to invest in them or not. 
>> 1. From the analysis The company wants to know: : <br>
    1. Which variables are significant in predicting the price of a house.<br>
    2. How well those variables describe the price of a house <br>

- Business Objectives :
>> You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.



## Model Building and Prediction
- Data Cleaning and analysis
> - Null value check and outliers treatment is performed on the data.
> - As part of EDA, pariplot and correlation heat map among variables is compared. Box plots compared for the categorical variables and regression plots for numerical variables.
- Data preparations
> - Dummy variables created using pandas.
> - Data is splited into train and test sets, using sckitl learn libraries
> - Data is splited into train and test sets, using sckitl learn libraries.

- Modelling the data
> - Recursive Feature Selection used to sort out primary significant features for the model.
> - Liner Regression model is fitted and stats predicted using Stats Models api.
> - Ridge and Lasso regression model fitted with cross validation
> - Optimal alpha values obtained and model fitted and used for prediction


## Conclusions
- Lasso model performed better than Ridge model on train and test data on a slight margin. Though we can not say that Ridge model is not performed well.
- Lasso model have better R2 score on test data, RSS and MSE error term are less on test data compared to Ridge Model.
- Lasso model optimizes the features and trimmed out 88 top important features from total of 218 features. Which increases the model efficiency.
- Optimal alpha value is 0.008 , which is also known as hyper parameter in case of regularization techniques.
- It explains 90% of variance present in the data correctly when tested on unknown data.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- library - PYTHON
- library - PANDAS
- library - NUMPY
- library - MATPLOTLIB
- library - STATSMODEL
- library - SKLEARN


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Contact
Created by [@Soumayad96] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->