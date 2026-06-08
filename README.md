# Plant Disease Detection Using EfficientNetB3

## Overview

This project implements a deep learning-based plant disease detection system using the EfficientNetB3 architecture. The model classifies plant leaf images into various disease categories and healthy classes, enabling early disease identification and supporting precision agriculture.

The project uses transfer learning, data augmentation, mixed precision training, and fine-tuning to achieve strong classification performance.

---

## Features

- Plant disease classification from leaf images
- Transfer learning with EfficientNetB3
- Data augmentation for improved generalization
- Mixed precision training for faster computation
- Fine-tuning of pretrained layers
- Evaluation using Accuracy, Precision, Recall, and F1-Score
- Prediction on unseen test images
- Visualization of training and validation performance

---

## Dataset

**Dataset:** New Plant Diseases Dataset (Augmented)

The dataset contains:
- Healthy plant leaves
- Multiple plant disease categories
- Thousands of labeled images

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn

---

## Model Architecture

- Base Model: EfficientNetB3 (Pretrained on ImageNet)
- Input Size: 192 × 192 × 3
- Data Augmentation:
  - Random Flip
  - Random Rotation
  - Random Zoom
  - Random Contrast
  - Random Translation
- Global Average Pooling
- Dense Classification Layer
- Softmax Output

---

## Training Strategy

### Phase 1: Feature Extraction
- Freeze EfficientNetB3 base layers
- Train custom classification head

### Phase 2: Fine-Tuning
- Unfreeze top layers of EfficientNetB3
- Continue training with a low learning rate
- Apply label smoothing to improve generalization

---

## Evaluation Metrics

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score

Training and validation curves are plotted to analyze performance and detect overfitting.

---

## Results

The trained model demonstrates strong classification performance on the validation dataset and effectively identifies plant diseases from leaf images.

Performance metrics include:

- Validation Accuracy
- Precision
- Recall
- F1-Score
- Per-Class Accuracy Analysis

---

## Future Improvements

- Deploy as a web application using Flask or Streamlit
- Mobile application for real-time disease detection
- Integration with agricultural advisory systems
- Support for additional crop species and diseases
- Explainable AI visualizations using Grad-CAM

---

## Applications

- Smart Farming
- Precision Agriculture
- Crop Health Monitoring
- Agricultural Research
- Disease Diagnosis Assistance

---

## Author

Siva Rama Krishna Namala

B.Tech Computer Science Student
Aspiring Software Engineer and Machine Learning Enthusiast