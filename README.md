# Fake News Detection
This project attempts to detect fake news. The dataset used for this project is gathered by Mr M. Zarharan.

## Features
Due to dataset parameters, the following features are extracted. A combination of these features is fed into a neural network to classify news as fake or truth.

### Featurs based on the background of the publisher in the dataset
- Correct_head
- Correct_body
- False_head
- False_body
- Cred_head
- Cred_body
- News source credibility 

### Features based on the publisher URL:
- web_host
- web_domain
- url
- transfer_protocol

### Stance of the claim in compare to news articles
- stance_a2c
- stance_h2c

For more details see [here](https://github.com/mahsaghn/Persian_Stance_Detection).

## Model Architecture
A simple 2 layer Neural Network with 30 and 2 nodes are used to classify news articles. `categorical_crossentropy` is used for loss function.

### Train Procedure
![alt text](https://github.com/mahsaghn/FakeNewsDetection/blob/main/acc.png)
![alt text](https://github.com/mahsaghn/FakeNewsDetection/blob/main/loss.png) 

The left figure illustrates the accuracy of the model during the training procedure and the right figure illustrates the loss value of the model after each iteration during the training procedure.

## OverSampling 
The proposed dataset is highly imbalanced. So it is not easy for the model to train features of the minor class. using oversampling methods help the model to train all labels. Consequently, the model will be more robust.  For more details see the section 'OverSampler' of [fakenews_v3.ipnb](https://github.com/mahsaghn/FakeNewsDetection/blob/main/fakenews_v3.ipynb). 

MIT license
