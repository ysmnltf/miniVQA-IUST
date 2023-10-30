# miniVQA Competition Solutions Repository

This repository contains my solutions to the [miniVQA](https://www.kaggle.com/c/minivqaiust) Kaggle competition. Below, you'll find a brief overview of each version.
Models are implemented using PyTorch library.

## Version 1

Question features are extracted using **Word2Vec or FastText Embeddings** and **LSTM layers**.
Image features are available in the dataset.
The question and image features are fused with **concatenation**.
The correct answer is predicted with a Dense layer.

**Best Validation Accuracy: 0.763**

## Version 2

Question features are extracted using **DistilBert**. In v2.2, I've tried fine-tuning the bert model on the dataset.
Image features are available in the dataset.
The question and image features are fused with **concatenation**.
The correct answer is predicted with a Dense layer.

**Best Validation Accuracy: 0.927**

## Version 3

Question features are extracted using **Word2Vec or FastText Embeddings** and **LSTM layers**.
Image features are available in the dataset.
The question and image features are fused with **cross-attention**. I've tried multihead attention and VIsualBert for this approach.
The correct answer is predicted with a Dense layer.

**Best Validation Accuracy: 0.881**

## Version 4

Question features are extracted using **DistilBert**.
Image features are available in the dataset.
The question and image features are fused with **cross-attention**. I've tried multihead attention for this approach.
The correct answer is predicted with a Dense layer.

**Best Validation Accuracy: 0.936**
