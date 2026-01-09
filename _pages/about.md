---
permalink: /about/
title: "About"
author_profile: true
redirect_from: 
  - /about.html
---

I am a software engineer at [White Hack Labs](https://whitehacklabs.com/) in New York, where I build AI-driven security tools for [HackerGPT](https://hackergpt.app/)—a platform serving 10,000+ users that detects breaches by identifying cross-modal inconsistencies across data signals.

I completed my **Master of Science in Data Science** from the [University at Buffalo](https://www.buffalo.edu/), where I also worked as a Research Assistant at the [Center for Unified Biometrics and Sensors (CUBS) Lab](https://www.buffalo.edu/cubs.html). My undergraduate degree is in Computer Science and Engineering from [The National Institute of Engineering](https://nie.ac.in/), Mysore, India.

---

## Research Vision

I propose developing **cross-modal world models** that learn physical properties through prediction discrepancy. The core insight: when a system predicts the deformation that should accompany applied pressure and observes a mismatch, that error reveals physical properties—elasticity, hardness, material authenticity—that neither modality encodes alone.

This prediction-error-as-physics principle, which I demonstrated in spoof detection, offers a path to AI systems that understand *how the world behaves*, not just what appears in a scene.

---

## Key Publication

**GestSpoof: Gesture-Based Spatio-Temporal Representation Learning for Robust Fingerprint Presentation Attack Detection**  
*IEEE 18th International Conference on Automatic Face and Gesture Recognition (FG 2024)*

Working with Prof. Srirangaraj Setlur at CUBS, I hypothesized that the discriminative signal in fingerprint spoof detection lies not in appearance but in dynamics. When pressure is applied, real skin and silicone respond differently—not because they look different, but because they behave differently.

I conceptualized and led the development of GestSpoof, introducing intentional distortion through gestures and fusing spatial features from ridge patterns with temporal features from minutiae displacement. Our architecture achieved **83.84% F1 score**—a 10% absolute improvement over the best static baselines.

[Paper](https://brosdocs.net/fg2024/027.pdf) | [Dataset](https://www.buffalo.edu/cubs/research/datasets/gestspoof-dataset.html)

---

## Research Directions

**Aim 1: Bidirectional Audio-Visual World Models for Material Property Inference**  
Extending motion→sound AND sound→motion prediction. When a system predicts the sound that should accompany visual deformation and observes a mismatch, the error vector encodes material properties.

**Aim 2: Temporal Cross-Modal Prediction for Action Dynamics**  
Train models to predict: given current visual state + action, what sound/visual change occurs? Action semantics emerge from prediction patterns.

**Aim 3: Cross-Modal Consistency for Authenticity Verification**  
Use cross-modal prediction error as anomaly detector for AI-generated content. Synthetic/manipulated content produces higher prediction error because it doesn't follow real-world physics.

---

## Skills

**Programming**: Python, C++, JavaScript, SQL  
**ML/DL Frameworks**: PyTorch, TensorFlow, OpenCV, scikit-learn  
**Tools**: Git, Docker, AWS, Linux  
**Research Areas**: Computer Vision, Cross-Modal Learning, Video Understanding, Biometric Security

---

## Contact

<a href="https://calendly.com/shreeramgs/video-interview" class="btn btn--primary"><i class="fas fa-calendar"></i> Schedule a Meeting</a>
<a href="mailto:shreeramgs666@gmail.com" class="btn btn--secondary"><i class="fas fa-envelope"></i> Email</a>
