# FakeNewsDetection
This porject attemps to detecet fake news. 

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

## Train Procedure
![alt text](https://github.com/mahsaghn/FakeNewsDetection/blob/main/acc.png)
![alt text](https://github.com/mahsaghn/FakeNewsDetection/blob/main/loss.png) 

The left figure illustrates the accuracy of the model during the training procedure and the right figure illustrates the loss value of the model after each iteration during the training procedure.
MIT license
