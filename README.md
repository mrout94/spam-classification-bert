# Spam Classification using NLP and BERT
Using Bert and 🤗 library to do basic binary text classification into spam or not-spam.  
This model achieves OOF ROC=0.99 and F1 Score=0.983.  
You can try and modify this notebook on [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Qf-eVyr1CGxtiO-SeqvLBVojOA_3jR3x?usp=sharing)

## Problem Statement
Given a group of sentences, we need to build a prediction model that will accurately classify which texts are spam.

## Data Description:-
* The SMS Spam Collection is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages in English of 5,574 messages, tagged acording being ham (legitimate) or spam.  
* This corpus has been collected from free or free for research sources at the Internet: [Link](https://www.kaggle.com/uciml/sms-spam-collection-dataset)  
* It is a very unbalanced dataset with a ratio of 87:13.

## Data Cleaning:-
Basic text cleaning procedures like removing emojis, web links, HTML tags, special charecters etc.

## Model
* This approach consists of a vanilla **bert-base-uncased** model finetuned on our dataset using **PyTorch**.
* I have also demonstrated the use for no-decay to improve model performance.
* Other Deep Learning concepts like Optimizer, scheduler, dropout etc have been covered with their implementation in Pytorch.

## Performance:-  
**ROC: 0.99  
F1: 0.983**
