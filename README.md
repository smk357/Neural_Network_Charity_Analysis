# Neural_Network_Charity_Analysis

### An analysis of charity funding status using neural networks

##Overview

The purpose of the project was to create a neural network model to predict successful charities funded. 

## Results

- The variable "Is_Successful" was the target variable
- The variables "EIN" (ID) and "NAME" were dropped as they were neither targer variables nor features
- The remaining data columns were features (43 inputs once the categorical variables were encoded)
- There 2 layers consiting of 85 and 50 neurons in each layer, with 3 total activation functions (relu for the 2 hidden layers and sigmoid for the output layer)
- The first pass through the testing data (accuracy of 69.62%) did not achieve the target accuracy of 75%:

![image](https://user-images.githubusercontent.com/79061124/126256807-d93f2b2a-6616-4d59-8857-0244a70d8038.png)

- Performance was improved by altering the binning on the 2 most variable categorical variables (application ID and classification ID) by selecting a lower density cutoff point, and increasing the number of neurons in the two hidden lawyers as well as the number of epochs. Accuracy reached 72.59% on the third attempt (hidden layer 1 neurons:150, hidden layer 2 neurons:100, and 250 epochs):

![image](https://user-images.githubusercontent.com/79061124/126257421-db900e8b-c8f3-4d85-9806-8015b60f043b.png)

## Summary

Overall, the neural netword model was able to predict charity success at an acceptable rate - over 70%.

