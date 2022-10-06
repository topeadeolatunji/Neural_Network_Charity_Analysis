# Neural Network Charity Analysis

## Overview

Alphabet Soup Charity, a non-profit company, needs help analyzing the impact of their donors' contribution and vetting potential charities by predicting which organizations are worth donating to and which of them are high risk. I designed a deep learning neural network that evaluates all types of input data and produces a clear decision making result using the Python TensorFlow library.

## Findings and Results

The IS_SUCCESSFUL column is considered the target for the model.
The APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT columns are considered to be the features of my model.
The EIN, NAME, STATUS, and SPECIAL_CONSIDERATION columns are neither targets nor features and should be removed from the input data.

Below is a screenshot of the code that preprocesses the data: 

<img width="953" alt="image" src="https://user-images.githubusercontent.com/104689265/194191696-5b02b5fa-87cc-464b-bb5f-4ccf3256057d.png">


## Compiling, Training, and Evaluating the Model

I selected 120 neurons with a sigmoid function for the first layer, 50 nuerons with a ReLU function for the second, and 18 neurons with for the third, and a sigmoid function for the outer layer. I only achieved an accuracy of 66% and was not able to achieve the target model performance of 75%. 

Desiging the model and creating a callback that saves the model's weights every 5 epochs: 

<img width="921" alt="image" src="https://user-images.githubusercontent.com/104689265/194192120-432515d2-12b6-46d3-99af-af5aaf17bd99.png">
<img width="763" alt="image" src="https://user-images.githubusercontent.com/104689265/194192242-9b1784f4-8b90-4778-92a1-8537507a6808.png">

## Summary & Conclusion

With the removal of noisy features, additional neurons and hidden layers and changed activation functions, the accuracy of my optimized model for predicting whether a donation is successful ended up being 0.6556 and its loss metric was 0.8546.

