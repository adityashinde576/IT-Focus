Binary Classification: Predicting Pass or Fail Using a Neural Network
Overview

This project demonstrates a simple binary classification task using a neural network. The goal is to predict whether a student will pass or fail based on the number of hours studied and the previous exam score. This serves as an introductory example of how deep learning can be applied to small structured datasets.

Objective

The main objectives of this project are:

To build a dataset with study-related features.

To train a neural network model that predicts Pass or Fail.

To apply data preprocessing techniques such as label encoding and feature scaling.

To evaluate the model's accuracy and test it on a new input example.

Dataset Description

The dataset contains three columns:

Hours_Studied

Previous_Score

Result (Pass or Fail)

These variables help determine a student's likelihood of passing based on effort and prior performance. The result column is converted into numeric form so that it can be used in model training.

Methodology
1. Data Preparation

A small dataset of ten entries is created. The features (Hours_Studied and Previous_Score) act as inputs to the model. The target variable (Result) is transformed into binary form where Fail corresponds to 0 and Pass corresponds to 1.

2. Train–Test Split

The dataset is divided into training and testing subsets. This helps evaluate how well the model generalizes to new data.

3. Feature Scaling

Standardization is applied to the input features. This ensures that each feature contributes equally during model training, improving training stability and performance.

4. Neural Network Model

A simple feed-forward neural network is constructed with:

One hidden layer for learning patterns.

An output layer with a sigmoid activation function for binary classification.

The model is trained using binary cross-entropy loss and the Adam optimizer.

5. Model Training

The model is trained for multiple epochs. During training, the network learns the relationship between the input features and the target class.

6. Model Evaluation

After training, the model is tested on unseen data. The accuracy score indicates how well the model predicts pass or fail outcomes on new students in the test set.

7. Prediction on New Input

A new student's data is scaled and passed to the model. The model outputs a probability indicating how likely the student is to pass. Based on the probability threshold, the prediction is classified as Pass or Fail.
