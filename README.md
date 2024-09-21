# Make-a-Thon
## Real Time Intrusion Detection using Deep Learning Techniques.
With the rapid expansion of the internet and increasing dependency on networked systems, network security has become a critical concern for organizations and individuals . Cyber attacks have grown in sophistication and frequency, posing significant threats to data integrity, confidentiality, and availability.To counter these threats, Intrusion Detection Systems(IDS) have been developed to monitor network traffic and identify malicious activities.
To enhance the performance of the Intrusion Detection System, we have implemented a Deep Learning Based Intrusion Detection System, using KDD CUP99 dataset.
It uses both Deep Neural Networks (DNN) and Recurrent Neural Networks (RNN) to classify network intrusions. The models are enhanced with Dropout regularization to prevent overfitting and improve performance. An ensemble model combines the predictions of both DNN and RNN for better accuracy. Evaluation metrics such as F1 score and ROC curves are used to assess model performance.
## Table of Contents
### 1.Dataset
### 2.Models
### 3.Evaluation Metrics

## Dataset
We use the KDD Cup 1999 dataset for building the intrusion detection system. The dataset is available in compressed format (kddcup.data_10_percent.gz). This dataset contains network traffic data labeled into different categories: normal and various attack types such as DOS attacks, probe attacks, etc.
### Features and Target Labels:
#### 1.Features: The dataset has 41 features representing various attributes of network connections.
#### 2.Target Labels: The target labels consist of different types of attacks and normal traffic.
For this project, the data is loaded and preprocessed to a suitable format for the neural networks.

## Models
### DNN Model
The Deep Neural Network (DNN) model is a feedforward network with multiple hidden layers. Dropout regularization is applied after each hidden layer to improve generalization and avoid overfitting.
It conitains an Input layer of 64 units of ReLU activation. Two Hidden Layers with 64, 32, and 16 units (ReLU activation) and an Output layer of Softmax activation with a number of neurons equal to the number of classes in the dataset.
#### Architecture:

##### Input layer: 64 units with ReLU activation.
##### Hidden layers: 3 fully connected layers with 64, 32, and 16 units (ReLU activation) and 50% dropout.
##### Output layer: Softmax activation with a number of neurons equal to the number of classes in the dataset.

### RNN Model 
The Recurrent Neural Network (RNN) model is built using LSTM (Long Short-Term Memory) units to capture temporal dependencies in the data. Dropout regularization is also applied to the LSTM layers.
#### Architecture:

##### Input layer: LSTM with 64 units (return sequences) and 50% dropout.
##### Hidden layer: LSTM with 32 units and 50% dropout.
##### Fully connected layer: 16 units (ReLU activation).
##### Output layer: Softmax activation with a number of neurons equal to the number of classes in the dataset.
