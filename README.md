# Seoul Bike Sharing Demand Prediction

![image](https://user-images.githubusercontent.com/102281845/190586017-c74bacd2-aee0-4589-bf05-32a9ccacaf58.png)

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# Introduction

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# Problem Statement

To predict the number of bikes rented each hour so  as to make an approximate estimation of the number of bikes to be made available to the public given a particular hour of the day.
![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)


# Data Description

The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information. Attribute Information: Date : year-month-day Rented Bike count - Count of bikes rented at each hour Hour - Hour of the day Temperature-Temperature in Celsius Humidity - % Windspeed - m/s Visibility - 10m Dew point temperature - Celsius Solar radiation - MJ/m2 Rainfall - mm Snowfall - cm Seasons - Winter, Spring, Summer, Autumn Holiday - Holiday/No holiday Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)
![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# Data Pre-processing and EDA

The exploratory data analysis and data pre-processing of this dataset has been successfully done and important inferences have been made from the obtained visualisations.
![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# Modelling and Conclusion

Linear regression model :  

MSE : 202937.66869256634

RMSE : 450.4860360683407

R2 : 0.5151094008043042

Adjusted R2 :  0.5117634047201476

Decision tree model :  

The best Decision Tree R2 score is 0.7753673960792731 with max depth 10.
The best R2 test score is : 0.7948642204947705 with max depth = 10 

Random forest model : 

The best Random Forest R2 train score is : 0.8278994903973604 with n estimators = 20, max depth : 15, min samples split : 4 and min samples leaf : 1 . 
The best Random Forest R2 test score is : 0.8516768166059918 with n estimators = 20, max depth : 15, min samples split : 4 and min samples leaf : 1

The most important features who had a major impact on the model predictions were; hour, temperature, Humidity, solar-radiation, and Winter.

The model performed well in this case but as the data is time dependent, values of temperature, wind-speed, solar radiation etc. will not always be consistent. Therefore, there will be scenarios where the model might not perform well. As Machine learning is an exponentially evolving field, we will have to be prepared for all contingencies and also keep checking our model from time to time.
