---
layout: post
title: A Deep Learning-based 3D position reconstruction for XENONnT
image: "/posts/cnn-fruit-classification-title-img.png"
tags: [Deep Learning, CNN, RNN, Data Science, Computer Vision, Python]
---

In this project I build & optimise a Convolutional Neural Network to reconstruct the three-dimensional position of an event within our detector that is used in the experiment XENONnT. I will also compare it with further model architectures, e. g. Recurrent Neural Networks. 

# Table of contents

- [00. Project Overview](#overview-main)
    - [Context](#overview-context)
    - [Actions](#overview-actions)
    - [Results](#overview-results)
    - [Growth/Next Steps](#overview-growth)
- [01. Data Overview](#data-overview)
- [02. Data Pipeline](#data-pipeline)
- [03. CNN Overview](#cnn-overview)
- [04. RNN Overview](#rnn-overview-main)
    - [LSTM](#rnn-overview-lstm)
    - [ConvLSTM2D](#rnn-overview-convlstm2D)
- [05. Tackling Overfitting With Dropout](#cnn-dropout)
- [06. Image Augmentation](#cnn-augmentation)
- [07. Hyper-Parameter Tuning](#cnn-tuning)
- [08. Transfer Learning](#cnn-transfer-learning)
- [09. Overall Results Discussion](#cnn-results)
- [10. Next Steps & Growth](#growth-next-steps)

___
