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
