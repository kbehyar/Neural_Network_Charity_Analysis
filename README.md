# Neural_Network_Charity_Analysis

## Overview of Project

### Purpose

This project is looking at creating a neural network model which will help by predicting whether applicants will be successful if funded by Alphabet Soup. 

## Results

### Data Preprocessing

- What variable(s) are considered the target(s) for your model?

The target variable is the "IS_SUCCESSFUL" column

- What variable(s) are considered to be the features for your model?

The features variables are the "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT" columns

- What variable(s) are neither targets nor features, and should be removed from the input data?

The variable that are not considered targets or features are the "EIN","NAME" columns

## Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

I chose 2 hidden layers, first layer includes 80 neurons and second includes 40 neurons. First two Hidden layers have the Relu activation function and the final out layer has the sigmoid activation function.

- Were you able to achieve the target model performance?

No, the target model performance of %75 was not achieved with the current model.

![](https://github.com/kbehyar/Neural_Network_Charity_Analysis/blob/main/Images/first%20sequential.PNG)

![](https://github.com/kbehyar/Neural_Network_Charity_Analysis/blob/main/Images/First%20accuracy.PNG)

![](https://github.com/kbehyar/Neural_Network_Charity_Analysis/blob/main/Images/First%20graph.PNG)



- What steps did you take to try and increase model performance?

1. First step taken was to add additional Hidden layers. I increased the layers from the original 3 to 5 layers. I started with 200 neurons on the first level and decreasing them by half for every layer after. 200 > 100 > 50 > 25. The results in this case did not change. The performance level decreased to %72.3

2. Second step was to reduce the Hidden layers to only one with 100 Neurons. Results continued to decrease the performance level.

3. Third attempt i reduced the number of Epochs for training. I also

4. Fourth i created more bins for rare occurrences in columns. I Increased the number of values for each bin for matters less than 1000.


![](https://github.com/kbehyar/Neural_Network_Charity_Analysis/blob/main/Images/Optimization%20attempt.PNG)

![](https://github.com/kbehyar/Neural_Network_Charity_Analysis/blob/main/Images/optimization%20accuracy.PNG)

![](https://github.com/kbehyar/Neural_Network_Charity_Analysis/blob/main/Images/optimization%20graph.PNG)




### Summary

My best results were achieved when i reduced the Hidden layers to 2, with 60 and 30 neurons each respectively. I used a Relu activation function for the hidden layers and sigmoid function for the output layer. I also Creating more bins for rare occurrences in columns. I Increased the number of values for each bin for matters less than 1000.

A random forest supervised learning model would have been more suitable for this type of data.
