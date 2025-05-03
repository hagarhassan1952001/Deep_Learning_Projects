# Binary Classification – Airline Delay Cause Prediction

This project is part of my Deep Learning practice. I built a binary classification model using TensorFlow and Keras to predict whether a flight will be *delayed* or *on time* based on various flight-related features.

## Overview

- *Type*: Supervised Binary Classification  
- *Goal*: Predict flight delay status  
- *Tools Used*: Python, Google Colab, TensorFlow/Keras, Scikit-learn, Pandas, Matplotlib  

## Dataset

The dataset used in this project is about *Airline Delay Causes*, which includes various features related to flights and their conditions.  
It aims to classify whether a flight will be delayed (1) or not (0).

- *Features include*:
  - Airline carrier  
  - Departure and arrival times  
  - Flight number  
  - Delay reasons (weather, security, NAS, late aircraft, etc.)  
  - And other relevant factors

- *Target*: Delay status (1 = Delayed, 0 = On-time)

## Model Architecture

A simple feedforward neural network using the Keras Sequential API:

python
Model(
    Input(shape=(17)),
    Dense(8,  activation = 'tanh'),
    Dense(128, activation = 'sigmoid'),
    Dense(64, activation = 'tanh'),
    Dense(32, activation = 'tanh'),
    Dense(1, activation = 'sigmoid')
)


- *Loss Function*: Binary Crossentropy  
- *Optimizer*: Adam  
- *Metric*: Accuracy

## Training

- *Epochs*: 100  
- *Batch Size*: 10000 

The model was trained using clean and scaled input data.

## Visualization

- Plots for training loss and accuracy  
- Decision boundary (if applicable)  
- Correlation heatmap for feature analysis (optional)

## How to Run

Open the notebook on Colab:

[Open in Google Colab](https://colab.research.google.com/drive/1yUtUjsmCXqMmMnUqdkgnG4seISPRsoy6)

Or view it on GitHub:

[View Notebook](https://github.com/hagarhassan1952001/Deep_Learning_Projects/blob/main/binary-classification/Binary_Classification_Mode.ipynb)

## Author

*Hagar Hassan*  
  [GitHub Profile](https://github.com/hagarhassan1952001)


