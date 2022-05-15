# Neural_Network_Charity_Analysis

## Overview of the analysis:

This project is an attempt to use neural network models to predict if applicants to a charity program would ne successful additions to the program. For this analysis a data set containing around 34,000 organizations that have been funded.

## Results:

* Data Preprocessing

1. The variable that was the target of the NN models was the IS_SUCCESSFUL column
2. All other variables were considered features for the model
3. Two variables where dropped (EIN and NAME) since they have little to no impact on the outcome.

* Compiling, Training, and Evaluating the Model

1. For the first pass of the model I used two hidden layers with the relu activation function and 80 and 30 nodes respectively for each layer over 30 epochs which attained accuracy of roughly 70%. For the next attempt I used 2 hidden layers with 1000 nodes using selu for their activation function and 30 nodes using leaky_relu function, when ran over 20 epochs I was able to obtain an accuracy of 69.5%. For the last pass of the model I tried 3 hidden layers with 1000(activation functiom selu), 100(activation functiom relu) and 10(activation functiom leaky_relu) over 20 epochs with an accuracy of 64%.
2. I was slightly shy of obtaining target performance for the model.
3. If I was to try and futher optimize the model I would try less complicated models over more epoch to try and get the accuracy about 75%.

## Summary:

I believe further exploration of the data and trimming the data of variables that have little or no impact on the desired outcome along with running the model for more epochs would possibly attain the desired performance from the NN model.