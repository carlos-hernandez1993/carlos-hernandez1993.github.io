---
layout: post
title: Flight Tickets - Machine Learning
---

Hypothetically, a group of Directors requested our services for the creation and constitution of a company related to the aeronautical field, intended exclusively for a Commercial Airline. The data was taken from Data World database.

In addition, the creation of a model that allows predicting the price of the flight ticket to different destinations from different places of origin, in order to be able to evaluate the benefits that
could give this business.

## Data

Data taken from Data World Database:

-2955 rows.

-No null values.

-7 categorical variables and 1 numerical variable.

-Variables: customer, number of travelers, ticket price(Pounds Sterling), ticket class, date, 114 cities of origin, 200 destination cities, 67 airlines.

## Base City Proposal for Operations Center

The airport with the highest number of travelers is Heathrow Airport(London).

![Getting Started](https://raw.githubusercontent.com/carlos-hernandez1993/images_machinelearning/main/images/imagen1.png)

## Correlation of Variables

It was possible to define the correlations between each of the variables and the target variable (ticket price). For this, the categorical variables were converted to numeric variables, by means of string replacement functions and Label Encoder.

It is observed that the most important variable with respect to the target is the type of ticket class. Likewise, low correlations were identified with respect to the other variables.

Heatmap between numerical features in order to see lineal coodependence.

![Getting Started](https://raw.githubusercontent.com/carlos-hernandez1993/images_machinelearning/main/images/imahen%2010.png)

## Models

Model Selected: Random Forest Regressor.

Gridsearch to find best values. Low computational cost.

Features: 

    - max_depth: 50
    
    -max_features: 2

    -n_estimators: 1000

Models not selected: Linear and Polynomial Regression, Gradient Boosting Regressor, Ada Boost Regressor, XGBoost.

## Conclusion

The Random Forest Regression model can predict ticket prices depending on the place of origin, destination, airline, month, day and class of the ticket.

## Code

To see more about code, you can see this: 

[Link display text - Document](https://github.com/carlos-hernandez1993/BOOTCAMP_MACHINE_LEARNING)
