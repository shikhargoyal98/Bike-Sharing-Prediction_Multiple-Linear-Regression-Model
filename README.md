# Bike-Sharing-Prediction_Multiple-Linear-Regression-Model

**Overview:**

BoomBikes, a US-based bike-sharing company, has been struggling with a significant decline in revenue due to the ongoing COVID-19 pandemic. With the aim of bouncing back as the economy recovers, BoomBikes is working on a strategic business plan to boost revenue post-lockdown. A key part of this plan involves understanding how the demand for bike-sharing services will evolve once the quarantine restrictions lift.

To gain insights, BoomBikes has partnered with a consulting firm to analyze the factors influencing bike demand in the American market. The goal is to identify which variables most significantly affect the demand for shared bikes and understand how well these factors can predict bike usage.

The company has collected a large dataset containing daily bike demand figures across the country, influenced by various factors like weather, seasonality, and user habits. The task at hand is to build a model that predicts bike demand based on these variables. This model will help BoomBikes adjust their business strategy and ensure they meet customer expectations when the market recovers. Additionally, it will provide valuable insights for expanding into new markets.

**Data Preparation:**

The dataset contains categorical variables such as 'weathersit' and 'season', which are represented by numeric codes (1, 2, 3, 4) but actually have no inherent order. These should be converted into categorical string values for accurate analysis. The dataset also includes a 'yr' column, indicating the years 2018 and 2019. Although it may seem trivial, this variable might be important as bike-sharing services have gained popularity over time, making it relevant for predicting future demand.

**Model Building:**

The dataset includes three columns related to bike usage: 'casual' (the number of casual users), 'registered' (the number of registered users), and 'cnt' (the total number of rentals, including both casual and registered users). The target variable for the model is 'cnt', as it represents the overall bike demand. The goal is to build a predictive model using these variables to understand demand patterns and inform BoomBikes' strategy.

=========================================
Dataset characteristics
=========================================	
	
- dteday : date
  
- season : season (1:spring, 2:summer, 3:fall, 4:winter)
  
- yr : year (0: 2018, 1:2019)
  
- mnth : month ( 1 to 12)
  
- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
  
- weekday : day of the week
  
- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
  
+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
  
- temp : temperature in Celsius
  
- atemp: feeling temperature in Celsius
  
- hum: humidity
  
- windspeed: wind speed
  
- casual: count of casual users
  
- registered: count of registered users
  
- cnt: count of total rental bikes including both casual and registered
