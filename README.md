# Fungal Image Classification using Deep Learning

## Overview

This project implements a deep learning-based system for classifying microscopic fungal images using multiple neural network architectures.

The system leverages:
- Transfer learning using ResNet101  
- Custom CNN architectures for baseline comparison  
- Data augmentation and preprocessing techniques  

The goal is to accurately classify fungal species and evaluate different model architectures for performance and generalization.

---

## Problem Statement

Classifying fungal infections from microscopic images is a challenging task due to:
- Subtle visual differences between fungal structures  
- Class imbalance in datasets  
- High similarity between certain fungal categories  

This project addresses the problem by:
- Classifying fungal images into multiple categories  
- Comparing deep learning models for performance  
- Evaluating generalization and overfitting behavior  

---

## Dataset

- Dataset: DeFungi  
- Total Images: 9,114  
- Classes: 5 (H1, H2, H3, H5, H6)  

The dataset includes:
- Microscopic fungal images  
- Labeled categories representing different fungal structures  
- Curated data suitable for deep learning tasks :contentReference[oaicite:0]{index=0}  

---

## System Architecture

Microscopic Images
- Data Preprocessing
- Image Resizing (224x224)
- Data Augmentation
- Feature Extraction (CNN / ResNet101)
- Classification Layer
- Fungal Class Prediction

---

## Approach

### Data Preprocessing
- Image resizing for model compatibility (224x224)  
- Normalization  
- Data augmentation  
- Handling class imbalance  

---

### Model Design

**ResNet101 (Transfer Learning)**
- Pre-trained on ImageNet  
- Fine-tuned for fungal classification  
- Deep architecture with residual connections  

**Custom CNN Models**
- model_A: simple baseline architecture  
- model_B: deeper CNN for improved feature extraction  

---

### Model Comparison

- ResNet101 → highest accuracy and best generalization  
- model_A → overfitting observed due to simplicity  
- model_B → improved balance but lower accuracy  

ResNet101 achieved the best performance due to:
- strong feature extraction capability  
- ability to handle complex image patterns  
- reduced overfitting compared to custom models :contentReference[oaicite:1]{index=1}  

---

## Results

- **ResNet101 Accuracy:** ~88% :contentReference[oaicite:2]{index=2}  
- model_A Accuracy: ~59.63%  
- model_B Accuracy: ~58.86%  

### Key Insight
> Transfer learning significantly improves performance on complex image datasets compared to training CNNs from scratch.

---

## Technologies Used

- Python  
- NumPy, Pandas  
- TensorFlow / Keras  
- PyTorch  
- Torchvision  
- PIL  

---

## Project Structure

├── fungal_classification.ipynb

├── README.md

---

## How to Run

1. Clone the repository:
`git clone https://github.com/EeshaKulkarni77/Fungal-Image-Classification.git`

2. Open the notebook:
`Fungal_Image_Classification.ipynb`

3. Run all cells  

---

## Key Takeaways

- Transfer learning improves performance on medical image datasets  
- Deep architectures like ResNet101 outperform simple CNNs  
- Class imbalance significantly affects model accuracy  
- Model comparison is essential for selecting optimal architecture  

---

## Future Improvements

- Improve performance on minority classes  
- Explore advanced architectures (Transformers, DenseNet)  
- Apply better imbalance handling techniques (focal loss)  
- Expand dataset for better generalization  

---

## Disclaimer

This project is a research prototype for fungal image classification and is intended for educational purposes, not for clinical diagnosis.
