# Neural_Network_Charity_Analysis

## Overview of Analysis


machine learning and neural networks

create a binary classifiers that is able to predict whether applicants will be successful if funded by Alphabet Soup.

over 34,000 organizations that have received funding from the company

Pandas, Scikit-Learn
TensorFlow

## Preprocessing Data for a Neural Network Model

What variable(s) are considered the target(s) for your model?
- The variable considered as the target was IS_SUCCESSFUL because it indicates whether the charity funding was used effectively.

What variable(s) are considered to be the features for your model?
- Variables considered to be features for the model were APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.

What variable(s) are neither targets nor features, and should be removed from the input data?
- EIN and NAME were neither targets nor featured and were removed from the input data.

## Compile, Train, and Evaluate the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

- Were you able to achieve the target model performance?
No

#### First attempt

![Original Model](https://user-images.githubusercontent.com/90656004/155061006-32c5f346-57ea-425e-80ac-f2c1d1d78c65.PNG)

Hidden layer 1: 80 neurons

Hidden layer 2: 30 neurons

Activation function: relu

Target model performance acheived: No, the model achieved 73.8% accuracy.

### What steps did you take to try and increase model performance?

#### Second Attempt: Add a third hidden layer

Addition of a third hidden layer with 10 neurons
![Optimization 1 Third Hidden Layer](https://user-images.githubusercontent.com/90656004/155060909-2a4c6e61-a7c4-4b52-ae5b-8754d23078e3.PNG)

Hidden layer 1: 80 neurons

Hidden layer 2: 30 neurons

Hidden layer 3: 10 neurons

Activation functions: relu for the hidden layers and sigmoid for the output layer

Target model performance acheived: No, the model achieved 74.2% accuracy.

#### Third Attempt: Add a third hidden layer and tanh activation function
Addition of a third hidden layer with 10 neurons and change the activation function from relu to tanh
![Optimization 2 Third Hidden Layer and Tanh Activation Function](https://user-images.githubusercontent.com/90656004/155060915-6e84c70b-cd86-44b6-b7b7-ecd851664eef.PNG)

Hidden layer 1: 80 neurons

Hidden layer 2: 30 neurons

Hidden layer 3: 10 neurons

Activation functions: tanh for the hidden layers and sigmoid for the output layer

Target model performance acheived: No, the model achieved 74.0% accuracy.

#### Fourth Attempt: Add a third hidden layer and more neurons
Addition of a third hidden layer and more neurons in the first and second hidden layers
![Optimization 3 Third Hidden Layer and More Neurons](https://user-images.githubusercontent.com/90656004/155060921-d5c2c7f9-b43c-4866-b1d7-d3630850144b.PNG)

Hidden layer 1: 80 neurons

Hidden layer 2: 50 neurons

Hidden layer 3: 30 neurons

Activation functions: relu for the hidden layers and sigmoid for the output layer

Target model performance acheived: No, the model achieved 74.0% accuracy.

## Summary
