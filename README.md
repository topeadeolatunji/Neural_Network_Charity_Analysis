# Neural Network Charity Analysis

## Purpose

A hypothetical nonprofit foundation, Alphabet Soup, needs help analyzing the impact of their donations and vetting potential recipients by predicting which organizations are worth donating to and which are too high risk. I designed a deep learning neural network that evaluates all types of input data and produces a clear decision making result using the Python TensorFlow library.

## Findings and Results

The IS_SUCCESSFUL column is considered the target for my model.
The APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT columns are considered to be the features of my model.
The EIN, NAME, STATUS, and SPECIAL_CONSIDERATION columns are neither targets nor features and should be removed from the input data.
Below is a screenshot of the code I wrote that preprocesses the data: 

Compiling, Training, and Evaluating the Model

I selected 120 neurons with a sigmoid function for my first layer, 50 nuerons with a ReLU function for the second, and 18 neurons with for the third, and a sigmoid function for the outer layer. I chose to change the activation function for the first layer because it increased the model's performance.
I only achieved an accuracy of 69% and was not able to achieve the target model performance.
I tried to increase the model performance by dropping more columns, creating more bins for rare occurances in columns, decreasing the number of values in some bins, adding more neurons to the hidden layers, using a differnet activation function, and increasing the number of epochs.
Below are screenshots of the code I wrote desiging the model and creating a callback that saves the model's weights every 5 epochs: 
 

## Summary & Conclusion

Through the removal of noisy features, additional neurons and hidden layers and changed activation functions, the accuracy of my optimized model for predicting whether a donation is successful ended up being 0.6868 and its loss metric was 1.3676.

A random forest model could solve this classification problem by randomly sampling the preprocessed data and building several smaller, simpler decision trees. Some benefits of using a random forest model include how robust it is against overfitting of the data because all of the weak learners are trained on different pieces of the data, it can be used to rank the importance of input variables, it is robust to outliers and nonlinear data, and it can run efficiently on large datasets.
