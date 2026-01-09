---
title: "Pneumonia Detection CNN"
excerpt: "Deep learning model using ResNet-50 for automated pneumonia detection from chest X-ray images. Achieves high accuracy for assisting radiologists in diagnosis."
collection: project
image: "/images/cnn_project.png"
tags:
  - Computer Vision
  - CNN
  - Medical AI
  - MXNet
github: "https://github.com/shreeramgs/pneumonia_detector"
---

# Pneumonia Detection from Chest X-Rays

This application uses convolutional neural networks to classify chest X-ray images for pneumonia detection. The model assists radiologists in predicting abnormalities with high accuracy.

## Model Architecture

- **Base Model**: ResNet-50 (pretrained on ImageNet)
- **Framework**: MXNet with GluonCV
- **Transfer Learning**: Fine-tuned for medical imaging

## Dataset

[Kaggle Chest X-Ray Dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)
- Normal vs Pneumonia classification
- Training, validation, and test splits

## Setup

```bash
pip install mxnet-cu101
pip install gluoncv
pip install comet-ml
```

## Features

- Automated X-ray classification
- Confusion matrix visualization via Comet.ml
- GPU acceleration support
- Transfer learning from ImageNet

## References

- [ResNet Paper](https://arxiv.org/abs/1603.05027)
- [GluonCV Transfer Learning Tutorial](https://gluon-cv.mxnet.io/build/examples_classification/transfer_learning_minc.html)
