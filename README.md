# Neural_Network_Charity_Analysis
## Overview
This project is going to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup using machine learning and neural networks, and eventually help the foundation predict where to make investments.

## Resources
Data Source: charity_data.csv<br/>
Software: Python 3.7.6 ,  Jupyter Notebook 6.4.8

## Results
### Preprocessing Data for a Neural Network Model
1.Preprocess the dataset before creating the neural network model, drop the non-beneficial columns, and create bins for rare occurrences in columns. <br/>
2.Encode categorical variables using one-hot encoding, split the preprocessed data into features and target arrays. <br/>
3.Split the preprocessed data into training and testing datasets, then scale the data.<br/>
- Q: What variable(s) are considered the target(s) for your model?<br/>
  A: The “IS_SUCCESSFUL” column is considered to be the target of my model.
- Q: What variable(s) are considered to be the features for your model?<br/>
  A: Every column except for the “IS_SUCCESSFUL” column are considered to be the target of my model.
- Q: What variable(s) are neither targets nor features, and should be removed from the input data?<br/>
  A: The “EIN” and “Name” columns should be removed from the input data.

### Compile, Train, and Evaluate the Model
Design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset, and then compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy.<br/>
- Q: How many neurons, layers, and activation functions did you select for your neural network model, and why?<br/>
  A: There are 80 neurons in layer 1, 30 neurons in layer 2, 1 neuron in the output layer, total 3 layers, within each layer, layer 1 and 2 use relu function, output layer use sigmoid function.
- Q: Were you able to achieve the target model performance?<br/>
  A: With an accuracy score of 0.725, I wasn’t able to achieve the target model performance of 75%.
- Q: What steps did you take to try and increase model performance?<br/>
  A: The steps I took to try to increase the model performance:<br/>
  - Attempt 1: Adding more neurons to a hidden layer
  - Attempt 2: Adding more hidden layers
  - Attempt 3: Using different activation functions for the hidden layers

## Summary
From the results above, the machine learning model ended up with an accuracy score of 72.6% after optimization, while the initial neural network had an accuracy score of 72.5%, so there is no significantly improvement after optimization as we can see.

