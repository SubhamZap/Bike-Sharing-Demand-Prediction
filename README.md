# Bike-Sharing-Demand-Prediction

Problem Statement: Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes. The objective of the project is to predict the hourly number of bikes rented for the stable supply of rented bikes.


Data Structure: We are provided with Seoul Bike Sharing Demand Prediction Dataset. The dataset contains around 8760 observations and 14 columns. Dataset having categorical and numerical features with any  null values and unwanted columns were removed which were of less importance.


Data Analysis: Seoul Bike prediction dataset contains variable like Date, Rented Bike Count, Hour, Temperature, Humidity, Windspeed, Visibility, Dew point temperature, Solar radiation, Rainfall, Snowfall, Season, Holiday and Functional day. Here our dependent variable was Rented bike count. 
With various visualization techniques, we got to understand the relationship of various variables like temperature, season, humidity, visibility, snowfall, etc. with our dependent variable. Using correlation heatmap, we found multi-collinearity among variables.
Various regression models like XGBoost, SVM, etc. were used to fit the data. Metrics like MAE, MSE, etc. were used to evaluate the performance of various models. Model with the highest r-squared score fits the data most accurately. Feature importance showed which features play most significant role in predicting the number of rented bikes.


Conclusion:

•	XGBoost Regression has given the best r2_score of 83.16% and with the least MAE, MSE, RMSE, MAPE errors.

•	Linear Regression doesn’t provide good fit of the data, so did Lasso. Ridge regression performance was even worse as it shrunk the parameters to reduce complexity.

•	Knn has performed better than Linear and Lasso regression.

•	SVM performs relatively well than KNN, as it can easily handle multiple continuous and categorical variables.

•	Features like days of no holidays, evening hours (17, 18, 19 and 20) and Autumn season plays important role in predicting the number of rented bikes.

