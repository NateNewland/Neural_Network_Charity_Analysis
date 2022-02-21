# Neural_Network_Charity_Analysis
## Project Overview
The purpose of this project is to use deep-learning neural networks with TensorFlow in Python, to analyze and classify the success of charitable donations.
We use the following methods for the analysis:
* preprocessing the data for the neural network model,
* compile, train and evaluate the model,
* optimize the model.
## Compliling and Evaluating
* This deep-learning neural network model is made of two hidden layers with 80 and 30 neurons respectively.
The input data has 43 features and 25,724 samples.
The output layer is made of a unique neuron as it is a binary classification.
To speed up the training process, we are using the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer.
For the compilation, the optimizer is adam and the loss function is binary_crossentropy.
* The model accuracy is under 75%. This is not a satisfying performance to help predict the outcome of the charity donations.
To increase the performance of the model, we applied bucketing to the feature ASK_AMT and organized the different values by intervals.
* We increased the number of neurons on one of the hidden layers, then we used a model with three hidden layers.
We also tried a different activation function (tanh) but none of these steps helped improve the model's performance.
## Summary
The deep learning neural network model did not reach the target of 75% accuracy. Considering that this target level is pretty average we could say that the model is not outperforming.
Since we are in a binary classification situation, we could use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.
