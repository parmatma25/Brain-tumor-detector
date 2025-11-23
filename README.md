# Brain-tumor-detector
Brain Tumor Classifier using VGG16 Transfer Learning. Classifies MRI scans into tumor subtypes (e.g., Glioma, Pituitary) using TensorFlow/Keras. Achieved ~84% accuracy.
# 🧠 Brain Tumor Detection System (BrainScan A.I.)

## Project Overview

This project develops a highly accurate **Convolutional Neural Network (CNN)** model designed to assist medical professionals by rapidly classifying brain tumors from MRI scans. The system functions as a robust digital assistant, capable of distinguishing between **Glioma, Meningioma, Pituitary, and No Tumor** with high confidence.

The primary objective was successfully achieved: building a model with a **validation accuracy exceeding 90%** on unseen data, mitigating the initial challenge of model overfitting.

---

## ✨ Features

The system includes three major functional modules:

1.  **Data Ingestion & Preprocessing:** Handles the input of raw MRI data, resizing, normalization (scaling pixel values to 0-1), and aggressive data augmentation (rotation, zooming, shifting) to ensure robust training.
2.  **Model Training & Optimization:** Initializes and trains a custom CNN architecture, utilizing **Dropout** and **L2 Regularization ($\lambda=0.005$)** to prevent overfitting.
3.  **Real-Time Classification:** Loads the trained model (`brain_tumor_detection_cnn.h5`) and outputs a definitive tumor classification along with a **confidence score** for any new MRI image.

## 💻 Technologies Used

| Category | Technology/Tool | Purpose |
| :--- | :--- | :--- |
| **Deep Learning Framework** | Python (3.x) | Core programming language |
| **Deep Learning Framework** | TensorFlow / Keras | Model definition, training, and prediction |
| **Scientific Computing** | NumPy | Efficient array manipulation and computation |
| **Development Environment** | Google Colab | Cloud-based training environment (used for GPU acceleration) |
| **Data Visualization** | Matplotlib | Plotting training history (Accuracy/Loss curves) |

---

## 🚀 Setup and Installation

### 1. Requirements

Ensure you have a working Python environment with the following libraries installed:

```bash
pip install tensorflow keras numpy matplotlib pillow
