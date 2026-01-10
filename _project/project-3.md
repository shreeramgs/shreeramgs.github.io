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

<div style="display: flex; justify-content: center; margin-bottom: 2em;">
  <div 
    style="
      background: #fff;
      border-radius: 16px;
      box-shadow: 0 2px 16px 0 rgba(0,0,0,0.17);
      padding: 2em 2em 1.5em 2em;
      max-width: 720px;
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
    "
  >
    <img 
      id="pneumonia-cnn-img"
      src="/images/cnn_project.png" 
      alt="Pneumonia Detection CNN" 
      style="max-width: 480px; width: 90%; height: auto; border-radius: 12px; box-shadow: 0 2px 8px 0 rgba(0,0,0,0.10); margin-bottom: 1em; transition: opacity 0.5s;"
    />
    <h2 style="margin: 0.5em 0 0.2em 0; font-size: 1.5em;">Pneumonia Detection CNN</h2>
    <p style="color: #444; margin: 0 0 0.5em 0; font-size: 1em; text-align: center;">
      Deep learning model using ResNet-50 for automated pneumonia detection from chest X-ray images. Achieves high accuracy for assisting radiologists in diagnosis.
    </p>
  </div>
</div>

### Description
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
