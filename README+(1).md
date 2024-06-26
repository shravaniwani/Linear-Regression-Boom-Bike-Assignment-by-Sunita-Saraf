# Boom Bike Assignment - Linear Regression

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
-  Project Description :
    The company wants to know:
    * Which variables are significant in predicting the demand for shared bikes.
    * How well those variables describe the bike demands
- Project Background : 
    * A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.. 
- What is the business probem that your project is trying to solve?
    * Create a model which will able to predict based on certain factors when the bike rental would be more
- What is the dataset that is being used?
    * Bike-rental data for time period 2018 to 2019

## Conclusions

Analysis is carried out using a Mixed Feature Selection Approach. 15 features are selected algorithmically using Recursive Feature Elimination. Further selection is done manually by looking at multicollinearity and statistical significance of features and overall fit of the model. The 10 most significant features to understand demand have been reported.

The data set is randomly divided into training and test data. Final Model built on training data set explains 84% of the variability and achieves 81% on test data.

The final relationship between demand and predictors is as follows.
- cnt = 1486.0791 + 1963.7864 yr + 70.766034 Saturday + 1280.737407 winter -614.119638 july -1063.6669 + workingday 35.500675 - -1253.070299 hum + 4234.263716 temp - -1008.319215 windspeed -1602.995038 light snow/rain 

where temp , windspeed and hum are normalized.

Note :
- Data has been cleaned to drop outliers that might affect the model adversely
- The model has been verified for Multicollinearity effects.
- Residual Analysis has been carried out and the model satisfies the assumptions of Linear Regression (Residuals follow a normal distribution, Errors exhibit homoscedasticity)
- plot between residual distribution shows that residuals follow a normal distribution for all interpolations. 
- Model is stable at 82%(+/-13%) coefficient of determination at 85% CI, ascertained through cross validation.
- Features in the order of influence has been reported by standardizing all predictor values.

## Technologies Used
- Matplotlib - v3.4.3
- Numpy   - v1.20.3
- Seaborn - v0.11.2
- Pandas  - v1.3.4
- sklearn
- statsmodels
- Python  - v3.9.7
- Excel
- Jupyter Notebook - v6.4.5
- IPython - v7.29.0
- Vscode - v1.67.0

## Acknowledgements

Contributer.
##Sunita Saraf

#### This project is created as part of IIITB and MultipleLinear regression assignment 
