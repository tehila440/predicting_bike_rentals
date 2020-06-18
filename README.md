## Predicting Bike Rentals

Communal bike sharing stations are located in many cities across the United States, including Washington D.C. One can rent these bicycles by the hour or by the day. We will be using data collected from the Washingtin D.C. bike share program. The data can be downloaded from the [University of California, Irvine's website](http://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset). This dataset contains the hourly and daily count of rental bikes between years 2011 and 2012 in Capital bikeshare system with the corresponding weather and seasonal information.

In this project we compare the following machine learning models:  Linear Regression, Decision Tree Regression, and Random Forest Regression. There is data cleaning, feature engineering, and hyperparamter optimization.  

GOAL: To predict the total number of bikes people rented (casual + registered) in a given hour. The cnt column is the target column. 

Random Forest performed the best out of the three methods.

Once we determined Random Forest Regression performed best we used that model to predict the casual rentals and registered rentals separately. 

The model is most accurate when using the casual rentals as the target column for predictions. If you look at the max value of the casual rentals it is 367 and the registered max is 886 rentals.  That is about 40% less rentals than the registered which could likely attribute to a smaller error.

Conclusion:  This is still a relatively small dataset. We are looking at only one city and one year's worth of data.  This project could be expanded to look at a larger date range.  We could also perform more feature engineering using weather and seasonal data.  