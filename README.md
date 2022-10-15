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
  ![initial neural network](https://user-images.githubusercontent.com/107179765/196010750-cecd97d8-e830-4313-99fa-3c384a6f398c.png)
- Q: Were you able to achieve the target model performance?<br/>
  A: With an accuracy score of 0.725, I wasn’t able to achieve the target model performance of 75%.
  ![initial neural network accuracy](https://user-images.githubusercontent.com/107179765/196010761-4f03a68b-f31f-4b44-bb14-9bfd182b9249.png)
- Q: What steps did you take to try and increase model performance?<br/>
  A: The steps I took to try to increase the model performance:<br/>
  - Attempt 1: Adding more neurons to a hidden layer
  ![attempt1](https://user-images.githubusercontent.com/107179765/196010803-1e313fd2-7e6a-4362-903f-c3398bf7478c.png)
  ![attempt1 accuracy](https://user-images.githubusercontent.com/107179765/196010808-7b59a8e7-e9e0-4b16-9361-54b9e2e55723.png)
  
  - Attempt 2: Adding more hidden layers
  ![attempt2 ong](https://user-images.githubusercontent.com/107179765/196010812-42d76986-b63c-4530-b8db-0a792bf676c7.png)
  ![attempt2 accuracy](https://user-images.githubusercontent.com/107179765/196010813-957c957f-351c-42a1-841f-6d8c02cf3002.png)
  
  - Attempt 3: Using different activation functions for the hidden layers
  ![attempt3](https://user-images.githubusercontent.com/107179765/196010818-0b60400c-120f-4cf1-b741-1b112a93c5ef.png)
  ![attempt3 accuracy](https://user-images.githubusercontent.com/107179765/196010823-4ed541b8-749c-4f4f-9531-63b98708daaf.png)

## Summary
From the results above, the machine learning model ended up with an accuracy score of 72.6% after optimization, while the initial neural network had an accuracy score of 72.5%, so there is no significantly improvement after optimization as we can see.

