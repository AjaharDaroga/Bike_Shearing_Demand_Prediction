# Bike_Shearing_Demand_Prediction
Capstone Project Supervised ML Regression :Seoul Bike Sharing Demand Prediction
Problem Description
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.
Data Description
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.
Attribute Information:
Date : year-month-day
Rented Bike count - Count of bikes rented at each hour
Hour - Hour of he day
Temperature-Temperature in Celsius
Humidity - %
Windspeed - m/s
Visibility - 10m
Dew point temperature - Celsius
Solar radiation - MJ/m2
Rainfall - mm
Snowfall - cm
Seasons - Winter, Spring, Summer, Autumn
Holiday - Holiday/No holiday
Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)


# Summary
The project goal is to minimize the waiting time or make rental bike available at the right time, so company want to predict the bike count required at each hour for the stable supply. Given dataset have past records of bike count during a day based on weather condition, season, holiday and functional day. For data preparation the categorical features convert by using one hot encoding or label encoding.
      Methodology for solving this problem is need to understand the data, prepare the data and visuals the data, important features selection and building a models finalize based on r2 score and root mean square error after that tune the hyperparameter.
     Performing exploratory data analysis on data to understand the how independent variable behavior with dependent variable. Checking multicollinearity because after plotting heatmap correlation we understood there are two independent variables strongly corelate with each other, so calculate the VIF then dropping the one of the features.  Most important features calculated based on information gain using mutual information from regression library, Important feature results have shown that temperature and hour of the day are most influence variable in hourly rented bike demand prediction.
    Budling the five different model Multilinear regression, Ridge regression, Decision tree, KNN, XGBoost model. Comparing the r2 score and root mean square error we get best score and low root mean square error from XGBoost model, but this model is behaving life back box model to understand how affecting the feature for final results we understand from shaply.
