# Bike Sharing Business Problem
> US bike-sharing provider BoomBikes in which bikes are made available for shared use to individuals on a short term basis for a price or free. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.
Essentially, the company wants —
- To identify variables which affect demand of shared bike
- To create a linear model that quantitatively relates demand of shared bikes with variables such as number of temperature, season etc.
- To know the accuracy of the model, i.e. how well these variables can predict demand of shared bikes.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)


## General Information
- Bike Sharing business problem is linear regression problem and two approaches are used for building linear regression model:
1.Manual Approach(without RFE)
2. Automatic Approach(with RFE)

In manual approach, all features are considered in model building. Therafter insignificants features are removed based on VIF value of features and p-value of co-efficients.

In automatic approach, RFE(Recursive Feature Elimination) is used for getting initial n significant features. Therafter insignificants features are removed based on VIF value of features and p-value of co-efficients.


## Conclusions
Final model is built with six(06) independet variables with 0.1024 RMSE(Root Mean Square Error) and R-squared value for test data and train data as 0.781 and 0.965 respectively.

- bikeDemand = 0.5597  x atemp + 0.2477  x  yr + 0.0537 x season + 0.0119 x weekday + 0.0321 x workingday - 0.0678 x weathersit
- Bike Demand is linearly dependent on feeling temperature, year, season, weekday, workingday and weather.


## Technologies Used
- library - Numpy 1.22.0
- library - Pandas 1.3.5
- library - Scikit-learn 0.22


## Contact
Created by [@harikrushn] - feel free to contact me!

