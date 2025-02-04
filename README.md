# Garbage Classification using CNN

This project demonstrates garbage classification using a Convolutional Neural Network (CNN) built with TensorFlow and Keras. The model is trained on a dataset of images of different types of garbage, and can be used to classify new images into these categories.


## Dataset

The dataset used for this project is the "Garbage Classification v2" dataset available on Kaggle. It contains images of 10 different types of garbage:

#### - battery
#### - biological
#### - brown-glass
#### - cardboad
#### - clothes
#### - green-glass
#### - metal
#### - paper
#### - plastic
#### - trash

The dataset is split into training and testing sets, with 80% of the data used for training and 20% for testing.


## Model

The CNN model used for this project consists of the following layers:

- Convolutional layer with 32 filters, a kernel size of (3, 3), and ReLU activation.
- Max pooling layer with a pool size of (2, 2).
- Convolutional layer with 64 filters, a kernel size of (3, 3), and ReLU activation.
- Max pooling layer with a pool size of (2, 2).
- Convolutional layer with 128 filters, a kernel size of (3, 3), and ReLU activation.
- Max pooling layer with a pool size of (2, 2).
- Flatten layer.
- Dense layer with 128 units and ReLU activation.
- Dropout layer with a rate of 0.5.
- Dense layer with 10 units (one for each class) and softmax activation.

The model is compiled with the Adam optimizer, categorical cross-entropy loss function, and accuracy metric.

