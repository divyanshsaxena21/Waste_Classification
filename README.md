# Garbage Classification using CNN

This project demonstrates garbage classification using a Convolutional Neural Network (CNN) built with TensorFlow and Keras. The model is trained on a dataset of images of different types of garbage and classifies them into these categories. In addition, the model classifies the waste into two broad categories: **recyclable** and **non-recyclable**.

## Dataset

The dataset used for this project is the "Garbage Classification v2" dataset available on Kaggle. It contains images of 10 different types of garbage:

#### - battery
#### - biological
#### - brown-glass
#### - cardboard
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
- Dense layer with 10 units (one for each class of garbage) and softmax activation.

### Recyclable vs Non-Recyclable Classification

In addition to classifying the specific types of garbage (such as paper, plastic, etc.), the model also classifies each image as **recyclable** or **non-recyclable**. This additional classification helps in streamlining the waste management process by automatically sorting waste into these two broad categories.

The model can therefore provide two types of outputs:
1. **Specific waste category** (e.g., cardboard, plastic)
2. **Recyclable/Non-recyclable** classification

## Model Compilation

The model is compiled with the following configurations:
- Optimizer: Adam
- Loss Function: Categorical Cross-Entropy (for classification of 10 waste types)
- Accuracy Metric: Accuracy

## Result

![image](https://github.com/user-attachments/assets/d673bdf7-f7c2-40ed-ba44-e091b5672c97)

The model successfully classifies the garbage images into their respective categories, and provides an additional classification of whether the waste is **recyclable** or **non-recyclable**.

