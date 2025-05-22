# CIFAR-10 Image Classification

A comprehensive machine learning project comparing traditional computer vision techniques with deep learning for CIFAR-10 image classification.

## 🎯 Overview

This project implements multiple approaches to classify CIFAR-10 images (10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck) using both traditional ML and CNN methods.

**Dataset:** 50,000 training + 10,000 test images (32×32 RGB)

## 🔧 Approaches

### Traditional Machine Learning
- **Feature Extraction:** Custom HOG + Color Histograms
- **Preprocessing:** MinMaxScaler + PCA (100 components)
- **Models:** KNN, Random Forest, SVM with GridSearchCV
- **Analysis:** Image transformation effects (blur, edge detection, sharpening)

### Deep Learning
- **CNN Architecture:** 3 conv blocks + dense layers with BatchNorm & Dropout
- **Training:** Adam optimizer, early stopping, 20 epochs
- **Performance:** Significantly outperforms traditional methods

## 📊 Key Features

- **Custom Implementations:** Manual HOG computation, convolution operations
- **Transformation Analysis:** Gaussian blur, Laplacian edge detection & sharpening
- **Model Persistence:** Saved models with joblib/HDF5
- **Comprehensive Evaluation:** Classification reports, confusion matrices, accuracy comparisons


## 📁 Project Structure

```
├── data/cifar-10-batches-py/
├── saved_models/          # Traditional ML models
├── saved_cnn_model/       # CNN model & history
├── main.py
└── README.md
```

## 📈 Results

| Method | Accuracy |
|--------|----------|
| Random Forest | ~0.5374% |
| SVM | ~0.6469% |
| KNN | ~0.5136% |
| **CNN** | **~ 0.8277%** |

**Transformation Effects:** Performance analysis under blur, edge detection, and sharpening transformations.

## 🛠️ Technical Highlights

- Manual HOG feature extraction with Sobel operators
- Custom convolution implementations for image transformations
- Systematic model comparison and hyperparameter tuning
- End-to-end pipeline from raw images to trained models


---

⭐ **Star this repo if you found it helpful!** ⭐
