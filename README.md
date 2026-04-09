# Cone Classification for Autonomous Racing

## Overview
This project focuses on classifying different types of cones used in autonomous racing events. The goal is to enable driverless vehicles to correctly identify track boundaries using machine learning techniques.

## Objective
- Classify four types of cones: Big Orange, Blue, Little Orange, and Yellow  
- Improve classification accuracy for real-time autonomous driving applications  
- Handle class imbalance and high-dimensional data effectively  

## Dataset
- Source: UniNa Corse Driverless Team  
- Derived from Formula SAE racing track videos  
- Images extracted using bounding boxes and labeled by cone type  
- Dataset consists of four classes with initial imbalance  

## Tools & Technologies
- Python (Jupyter Notebook, Anaconda)  
- Scikit-learn  
- NumPy, Pandas  
- OpenCV (for preprocessing)  
- Pre-trained datasets: ResNet34, EfficientNet  

## Methodology

### Data Preprocessing
- Combined and cleaned datasets  
- Removed irrelevant columns and checked for missing/duplicate values  
- Normalized and prepared data for training  

### Handling Class Imbalance
- Applied downsampling to balance all four cone classes  
- Ensured equal representation across categories  

### Feature Engineering
- Applied PCA (Principal Component Analysis)  
- Reduced dimensionality and extracted key latent features  

### Model Development
- Trained multiple models:
  - Support Vector Machine (SVM)  
  - Random Forest  
- Evaluated models on both ResNet34 and EfficientNet datasets  

## Results

| Dataset       | Random Forest | SVM | SVM + PCA |
|--------------|--------------|-----|----------|
| EfficientNet | 73%          | 84% | 85%      |
| ResNet34     | 92%          | 94% | 96%      |

- Best performance achieved: **96% accuracy (SVM + PCA on ResNet34 dataset)**  

## Key Features
- High classification accuracy using optimized ML pipeline  
- Effective handling of class imbalance  
- Improved model performance using PCA  
- Comparison across multiple datasets and models  

## Applications
- Autonomous driving systems  
- Driverless racing competitions  
- Object detection and classification tasks  

## Future Work
- Integration with real-time perception systems  
- Testing with deep learning models (CNNs)  
- Improving dataset diversity and robustness  

## Author
Sudip Kishan Sarker  
MSc Autonomous Vehicle Engineering  
University of Naples Federico II
