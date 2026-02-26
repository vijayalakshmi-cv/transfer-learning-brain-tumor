# transfer-learning-brain-tumor
# Transfer Learning for Brain Tumor Classification (MRI)

## Overview
This repository contains implementation of transfer learning–based deep learning models for brain tumor classification using MRI images.

The study evaluates multiple pre-trained CNN architectures to determine optimal performance on small medical imaging datasets.

## Dataset
- Modality: MRI (2D slice-based)
- Total images: 253
- Augmented to: 1000 samples
- Classes: Tumor / No Tumor
- Preprocessing:
  - Image resizing
  - Normalization
  - Data augmentation (rotation, shear, scaling)

> Note: Dataset not included due to size/privacy constraints.

---

## Model Architectures Evaluated
- VGG16
- VGG19
- ResNet50
- EfficientNetB0
- InceptionV3 (Best Performance – 94% accuracy)

Transfer learning strategy:
- Frozen convolutional base
- Custom classification head
- Dropout regularization
- Softmax output layer

---

## Training Configuration
- Framework: TensorFlow / Keras
- GPU: NVIDIA Tesla T4 (Google Colab)
- Batch size: 32
- Epochs: 100
- Optimizer: RMSprop / Adam
- Loss: Categorical Cross-Entropy
- Train/Test Split: 70/30

---

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Best Performing Model:
- InceptionV3 – 94% accuracy

---

## Repository Structure
