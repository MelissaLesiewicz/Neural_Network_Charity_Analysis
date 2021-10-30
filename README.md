# Neural_Network_Charity_Analysis
## Overview
From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.
Use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The dataset contains the following data:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

## Results:
### Data Preprocessing:
The target variable is the IS_SUCCESSFUL column values (0/1), we are trying to build a model that can predict successful venture for future funding.
Feature Variables are:
*  Application Type
*  Affiliation
*  Classification
*  Use Case
*  Status
*  Income Amount
*  Special Considerations
*  Ask Amount

Removed Variables(no impact on success of project):
*  EIN
*  Name

### First Model 
Compiling, Training, and Evaluating the Model
For the first model I tried 2 hidden layers. The first layer contained 88 neurons  (numbers of features times 2). The second layer I selected 44 neurons because it's half of the first layer. I used the relu activation function for the hidden layers and sigmoid for the output layer because it the standard for a starting point. Sigmoid it the traditional activation function for a classification problem.
This model had an accuracy rate of about 74.2% on the training data and 72.3% on the testing data.

To try and increase the model's perfomance I added added another bin to the application type category and another bin to the classification category. I added another hidden layer with 22 neurons becuase it is half of the second layer.
This did not increase performance.
In the third attempt I tried increasing the number of neurons to 132 (3x the number of inputs), with layers 2 and 3 having half the neurons of the layer before it. 
This increase performance only slightly. 

## Summmary
This model is only moderately accurate. Neural networks are designed to solve really complicated problems, a simpler classification model may be better suited to this binary classification problem. 

What steps did you take to try and increase model performance?
