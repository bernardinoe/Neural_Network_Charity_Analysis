# Neural Network Charity Analysis

## Overview of the analysis: Explain the purpose of this analysis.
The purpose of this analysis is to predict weather applicants will be succesful if funded by Alphabet Soup

## Results: Using bulleted lists and images to support your answers, address the following questions.

### Data Preprocessing

- What variable(s) are considered the target(s) for your model?
IS_SUCCESSFUL

- What variable(s) are considered to be the features for your model?
APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

- What variable(s) are neither targets nor features, and should be removed from the input data?
EIN and NAME

![A1](https://github.com/bernardinoe/Neural_Network_Charity_Analysis/blob/main/application_df.PNG)
![A2](https://github.com/bernardinoe/Neural_Network_Charity_Analysis/blob/main/application_df2.PNG)

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
first hidden layer: 80 units, activation = relu
second hidden layer: 30 units, activation = relu
output layer: 1 unit, activation = sigmoid

![nn](https://github.com/bernardinoe/Neural_Network_Charity_Analysis/blob/main/nn.PNG)

- Were you able to achieve the target model performance?
No, Performance is above 70% but not above 75%

![Result1](https://github.com/bernardinoe/Neural_Network_Charity_Analysis/blob/main/results1.PNG)

- What steps did you take to try and increase model performance?
I try to remove an additional variable. Addditionally, I tried using diferenc activations, and adding an additional layer.

Accuracy per Attempt

Attempt 1: 0.7227988243103027
![Attempt1](https://github.com/bernardinoe/Neural_Network_Charity_Analysis/blob/main/Attempt1.PNG)

Attempt 2: 0.7210495471954346
![Attempt2](https://github.com/bernardinoe/Neural_Network_Charity_Analysis/blob/main/Attempt2.PNG)

Attempt 3: 0.719650149345398
![Attempt3](https://github.com/bernardinoe/Neural_Network_Charity_Analysis/blob/main/Attempt3.PNG)


## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
It was difficult to reach an accuracy of more 75% or more. The more i tried to increase performance, the lower number I would get. I would use the random forest model as it can handle a bigger dataset, use less time, avoids overfitting and has a better accuracy than other models.