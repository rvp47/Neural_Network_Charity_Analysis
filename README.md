# Neural_Network_Charity_Analysis

## Overview of Analysis

Alphabet Soup is a charitable organization that has funded more than 34,000 organizations over the years. Machine learning and neural networks were used in this analysis to create a binary classifier that is able to predict whether applicants will be successful if funded by Alphabet Soup. The target model performance is 75%. To attempt to achieve this accuracy score, various optimization methods were employed, including changing the number of neurons, number of hidden layers, and the type of activation function.

## Preprocessing Data for a Neural Network Model

What variable(s) are considered the target(s) for your model?
- The variable considered as the target was IS_SUCCESSFUL because it indicates whether the charity funding was used effectively.

What variable(s) are considered to be the features for your model?
- Variables considered to be features for the model were APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.

What variable(s) are neither targets nor features, and should be removed from the input data?
- EIN and NAME were neither targets nor featured and were removed from the input data.

## Compile, Train, and Evaluate the Model

#### Initial attempt

![Original Model](https://user-images.githubusercontent.com/90656004/155061006-32c5f346-57ea-425e-80ac-f2c1d1d78c65.PNG)

How many neurons, layers, and activation functions did you select for your neural network model, and why?
- Hidden layer 1: 80 neurons
- Hidden layer 2: 30 neurons
- Activation function: relu

Were you able to achieve the target model performance?
- No, the model achieved 73.8% accuracy.

### What steps did you take to try and increase model performance?

#### First Optimization Attempt: Add a third hidden layer with 10 neurons
![Optimization 1 Third Hidden Layer](https://user-images.githubusercontent.com/90656004/155060909-2a4c6e61-a7c4-4b52-ae5b-8754d23078e3.PNG)

How many neurons, layers, and activation functions did you select for your neural network model, and why?
- Hidden layer 1: 80 neurons
- Hidden layer 2: 30 neurons
- Hidden layer 3: 10 neurons
- Activation functions: relu for the hidden layers and sigmoid for the output layer

Were you able to achieve the target model performance?
- No, the model achieved 74.2% accuracy.

#### Second Optimization Attempt: Add a third hidden layer with 10 neurons and tanh activation function
Addition of a third hidden layer with 10 neurons and change the activation function from relu to tanh
![Optimization 2 Third Hidden Layer and Tanh Activation Function](https://user-images.githubusercontent.com/90656004/155060915-6e84c70b-cd86-44b6-b7b7-ecd851664eef.PNG)

How many neurons, layers, and activation functions did you select for your neural network model, and why?
- Hidden layer 1: 80 neurons
- Hidden layer 2: 30 neurons
- Hidden layer 3: 10 neurons
- Activation functions: tanh for the hidden layers and sigmoid for the output layer

Were you able to achieve the target model performance?
- No, the model achieved 74.0% accuracy.

#### Third Optimization Attempt: Add a third hidden layer and more neurons overall
Addition of a third hidden layer and more neurons in the first and second hidden layers
![Optimization 3 Third Hidden Layer and More Neurons](https://user-images.githubusercontent.com/90656004/155060921-d5c2c7f9-b43c-4866-b1d7-d3630850144b.PNG)

How many neurons, layers, and activation functions did you select for your neural network model, and why?
- Hidden layer 1: 80 neurons
- Hidden layer 2: 50 neurons
- Hidden layer 3: 30 neurons
- Activation functions: relu for the hidden layers and sigmoid for the output layer

Were you able to achieve the target model performance?
- No, the model achieved 74.0% accuracy.

## Summary
Despite several attempts to optimize the model, it was not able to achieve the target model performance of 75%. The accuracy scores achieved were between 73.8% and 74.2%. The model that acheived the highest accuracy had a third hidden layer with 10 neurons, a relu activation function for the hidden layers, and a sigmoid activiation function for the output layer.

For future analysis, it is recommended that the Random Forest Classifer be used to solve this classification problem. This supervised machine learning model is capable of combining many decision trees to generate a classified output, having a faster performance, and avoiding overfitting the data.
