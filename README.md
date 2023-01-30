# Neural Network Charity Analysis

## Overview 

The purpose of this analysis is to measure if applicants will be successful if funded by Alphabet Soup by creating a binary classifier.  Deep neural network model was designed to complete analysis.  The data format is CSV with more than 34,000 organizations that have received funding from Alphabet Soup over the years.  The dataset contains the metadata metadata about each organization, such as the following:
   
Within this dataset are a number of columns that capture 

- EIN and NAME—Identification columns

- APPLICATION_TYPE—Alphabet Soup application type

- AFFILIATION—Affiliated sector of industry

- CLASSIFICATION—Government organization classification

- USE_CASE—Use case for funding

- ORGANIZATION—Organization type

- STATUS—Active status

- INCOME_AMT—Income classification

- SPECIAL_CONSIDERATIONS—Special consideration for application

- ASK_AMT—Funding amount requested

- IS_SUCCESSFUL—Was the money used effectively

## Results: 

Data Preprocessing

- What variable(s) are considered the target(s) for your model?

    IS_SUCCESSFUL

- What variable(s) are considered to be the features for your model?

    APPLICATION_TYPE

    AFFILIATION—Affiliated

    CLASSIFICATION

    USE_CASE

    ORGANIZATION

    STATUS

    INCOME_AMT

    SPECIAL_CONSIDERATIONS

    ASK_AMT

- What variable(s) are neither targets nor features, and should be removed from the input data?

    EIN and NAME

Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

    

- Were you able to achieve the target model performance?

    No.  It did not achieved the target predictive accuracy higher than 75%. 

- What steps did you take to try and increase model performance?

    The following three steps were taken to increase model performance.

    1. Adjusting the input data to ensure that there are no variables that are causing confusion in the model.

    * Dropped one column, SPECIAL_CONSIDERATIONS

    * Created more bins for CLASSIFIACTION column by reducing the cutoff count from 2,000 to 1,000.
    
    2. Adding the third hidden layers.

    3. Adding the number of epochs from 50 to 100 to the training regimen.

## Summary: 

Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
There is a summary of the results (2 pt)
There is a recommendation on using a different model to solve the classification problem, and justification (3 pt)





