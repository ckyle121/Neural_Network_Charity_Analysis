# Neural Network Charity Analysis
## Overview / Purpose
The goal of this project is to use a type of machiene learning, neural network analysis, to determine the impact of charitable donations. When giving money to various organizations, it is important to determine which donations will bring a positive return on the investment. Through a series of filtering through various input data, this neural network will determine which organizations will be impactful after receiving a donation. 

## Results 
### Data Preprocessing 
-The target for this model is to determine the output of the column "Is_Successful." The goal is to recieve a return on investment, therefore, we want to advise to donation to charities that return "yes" for Is_Successful.

-The features of this model include "Application_Type" and "Classification." Because of their ability to group various charitable causes, which will determine what groups of causes result in positive outcomes.

-Columns that are neither features nor targets include description of identification attributs such as the "Name" and "EIN" which are specific to each individual row, and they do not help us when grouping alike chairities. 

### Compiling, Training, and Evaluating the model 
-The orignial model had two hidden layers and an output layer, however, I added a thrid hidden layer to attempt to improve accuracy. The neuron count his high around 100, 50, and 25 for each layer due to the large amount of data. 

-The target model performance was above 75%, however, the created model only returns a prediciton of 61%. After making my own adjustments to the model to attempt to iprove the accuracy score, I saw a decrease in accuracy which was not the goal of the target model.

-In order to try and improve the accuracy score, I tried 3 different solutions. The first thing I added was an extra hidden layer. Typically, adding another layer filters the data an additional time and improves accuracy; however, my score decreased by almost 10% when adding a third hidden layer. Secondly, I increased the number of neurons per layer to increase specificity in layers, attempting to narrow down the data. Finally, I dropped more idenitficaiton columns about each independent organizations such as organization, use case, and speical consdierations because these are identifiers and do not group to be helpful determining success. 

## Summary 
If I were to work with this same data again, I would attempt to use a classification model such as a Logisitic Regression because the data seems to be able to be split linearally. A logistic regression would create a binary for the data to determine whether or not the charity would return positively based on Application Type and Classification.
