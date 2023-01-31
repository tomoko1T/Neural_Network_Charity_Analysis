# Neural Network Charity Analysis

## Overview 

The purpose of this analysis is to predict wether applicants will be successful if funded by Alphabet Soup by designing the deep neural network model.  The type of classification for this research is a binary classification.  The data format is CSV with more than 34,000 organizations that have received funding from Alphabet Soup over the years.  The dataset contains the metadata metadata about each organization, such as the following:

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
 
### Data Preprocessing

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

### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

The number of neurons and layers show in the table below.   ReLu Activation was chosen for the hidden layers because it is a suitable activation function for multilayer perceptron.  For output layer, Sigmoid activation function was selected because this analysis was conducted to predict binary classification with one node.

![This is an image]() 

- Were you able to achieve the target model performance?

    No.  It did not achieved the target predictive accuracy higher than 75%. 

- What steps did you take to try and increase model performance?

    The following three steps were taken to increase model performance.

    1. Adjusting the input data to ensure that there are no variables that are causing confusion in the model.

    * Dropped one more column, SPECIAL_CONSIDERATIONS

    * Created more bins for CLASSIFIACTION column by reducing the cutoff count from 2,000 to 1,000.
    
    2. Adding the third hidden layers.

    3. Adding the number of epochs from 50 to 100 to the training regimen.

## Summary: 

The target predictive accuracy on both the original and optimization did not reach higher than 75%.  The results of each modeul is as follows:

### Original deep learning model

![This is an image]() 

Accuracy: 72%

Loss matric: 56%

The code is found [GitHub Pages](https://github.com/tomoko1T/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.ipynb)

### Optimization deep learning model 

![This is an image]() 

Accuracy: 72 %

Loss matric: 57%

The code is found [GitHub Pages](https://github.com/tomoko1T/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimization.ipynb)

The recommendation is to employ the random forest model because it is very similar to the neural network model.  Since the dataset format is tablular, it could worth to use this model to improve the accuracy. 
