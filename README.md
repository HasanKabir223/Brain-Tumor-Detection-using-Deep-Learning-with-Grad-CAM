# Brain Tumor Detection using Deep Learning with Grad-CAM

## Overview

This project focuses on **automatic brain tumor detection from MRI images** using deep learning, with an emphasis on **model interpretability** through **Grad-CAM (Gradient-weighted Class Activation Mapping)**.

The goal is not just classification accuracy, but also **understanding *why* the model makes a decision**, which is critical in medical AI applications.

This repository demonstrates:

* End-to-end CNN-based tumor classification
* Proper medical image preprocessing
* Explainable AI using Grad-CAM
* Practical, production-oriented ML thinking

---

## Problem Statement

Manual analysis of brain MRI scans is:

* Time-consuming
* Prone to inter-observer variability
* Hard to scale in low-resource settings

This project attempts to assist radiologists by:

* Automatically detecting brain tumors
* Highlighting **important regions** in MRI scans using Grad-CAM

⚠️ **Disclaimer:** This project is for research and educational purposes only. It is **not** a medical diagnosis tool.

---

## Dataset

* Brain MRI images (glioma / meningioma / pituitary / No Tumor)
* Images resized and normalized
* Dataset split into training and test sets

## Model Architecture

* Convolutional Neural Network (CNN)
* Multiple convolution + pooling layers
* Fully connected classifier head
* Trained using Categorical Cross-Entropy loss

Key design choices:

* Balance between performance and interpretability
* Avoiding over-parameterization

---

## Grad-CAM Explainability

Grad-CAM is used to:

* Visualize **class-discriminative regions**
* Ensure the model focuses on tumor regions instead of noise
* Improve trust and transparency

### Why Grad-CAM?

* Model-agnostic
* Works directly with CNN feature maps
* Widely accepted in medical imaging research

Output:

* Heatmaps overlaid on original MRI images
* Clear focus on tumor regions in positive cases

---

## Results

* High classification accuracy on test data
* Grad-CAM heatmaps align well with tumor regions
* Minimal overfitting observed

---

## Project Structure

```
├── result
├── notebooks/
├── gradcam/
└── README.md
```
---

## Key Learnings

* Importance of explainability in healthcare AI
* Practical CNN design decisions
* Debugging and training stability
* Translating theory into real-world ML systems

---

## Author

**Hasan Kabir**
AI Engineer

---

## Final Note

This project reflects a **first-principles approach** to AI — focusing on *why models work*, not just *making them work*.

