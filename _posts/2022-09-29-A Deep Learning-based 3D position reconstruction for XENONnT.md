---
layout: post
title: A Deep Learning-based 3D position reconstruction for XENONnT
image: "/own_projects/tpc.png"
tags: [Deep Learning, CNN, RNN, Data Science, Computer Vision, Python]
---

In this project I build & optimise different kinds of neural networks to reconstruct the three-dimensional position of an event within our detector that is used in the experiment XENONnT. The goal is especially the reconstruction of the depth of an event in the detector, because this can be determined by conventional methods only by the time difference of 2 signals, a more detailed description will be given later.

# Table of contents

- [00. Project Overview](#overview-main)
    - [The XENONnT experiment](#overview-xenonnt)
    - [Position reconstruction for XENONnT](#overview-posrec)
    - [Results](#overview-results)
    - [Growth/Next Steps](#overview-growth)
- [01. Data Overview](#data-overview)
- [02. Data Pipeline](#data-pipeline)
- [03. CNN Overview](#cnn-overview)
- [04. RNN Overview](#rnn-overview-main)
    - [LSTM](#rnn-overview-lstm)
    - [CNN-LSTM](#rnn-overview-cnnlstm)
- [05. Tackling Overfitting With Dropout](#cnn-dropout)
- [06. Image Augmentation](#cnn-augmentation)
- [07. Hyper-Parameter Tuning](#cnn-tuning)
- [08. Transfer Learning](#cnn-transfer-learning)
- [09. Overall Results Discussion](#cnn-results)
- [10. Next Steps & Growth](#growth-next-steps)

___

# Project Overview  <a name="overview-main"></a>

More is unknown than is known. It turns out that only about 5 % of the universe is baryonic matter. The rest is composed of dark matter and dark energy, which are invisible but dominate the structure and evolution of the universe. Determining the nature of dark matter, which accounts for much of the mass of galaxies in the universe, has been and remains one of the greatest puzzles of recent decades. The XENONnT eperiment, located in the underground laboratory Laboratori Nazionali del Gran Sasso (LNGS) in  Italy is looking for this dark matter, more specifically WIMPs, a dark matter candidate that has received a lot of attention recently.
