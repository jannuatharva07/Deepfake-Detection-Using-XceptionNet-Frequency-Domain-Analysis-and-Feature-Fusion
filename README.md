# Deepfake-Detection-Using-XceptionNet-Frequency-Domain-Analysis-and-Feature-Fusion(In progress)
Deepfake video detection model combining XceptionNet and Frequency Domain Analysis with feature fusion for improved authenticity verification.

# 1. Introduction
Deepfakes are AI-generated synthetic media in which a person’s likeness is replaced with someone else’s, making it difficult to distinguish between real and fake videos. With the rapid advancement of deep learning, deepfakes have become more realistic — posing serious challenges to security, privacy, and digital trust.

This project, “Deepfake Detection using Deep Learning (XceptionNet + Frequency Domain Analysis + Feature Fusion)”, aims to accurately identify fake images by combining spatial and frequency domain features. The model integrates XceptionNet (for image feature extraction) with Frequency Domain Analysis (FDA) and a Feature Fusion mechanism to enhance classification performance.

The system processes images to detect faces, extracts frames, and analyzes both visual and frequency cues to classify each video as Real or Fake. The approach leverages deep learning’s power for robust detection, even under heavy compression or visual manipulation.

# 2. Datasets
## 📊 Dataset Information

We used publicly available benchmark datasets to train and test the deepfake detection model.

- **FaceForensics++ (c40 compressed)**  
  Contains real and manipulated videos generated using multiple deepfake methods such as DeepFakes, FaceSwap, and Face2Face.  
  📎 [Download Link](https://drive.google.com/your_dataset_link)

- **DeepFakeDetection Dataset (DFD)**  
  Provided by Google, containing real and fake videos for training deepfake classifiers.  
  📎 [Download Link](https://drive.google.com/your_dataset_link)

Each video was processed using OpenCV and MTCNN for:
- Frame extraction  
- Face detection and cropping  
- Data normalization and resizing  

The combined dataset was used for training and validation.

## 🧩 Model Information

### 🧠 Model Components
1. **XceptionNet** – Used for spatial feature extraction from facial regions.  
2. **Frequency Domain Analysis (FDA)** – Extracts frequency features to capture hidden artifacts in fake images.  
3. **Feature Fusion** – Combines both spatial and frequency features for improved accuracy.  
4. **Classifier** – Final dense layers for binary classification (Real / Fake).

### 📁 Model Code Files
- `src/xceptionnet.ipynb` → XceptionNet implementation  
- `src/fda_feature_fusion.ipynb` → Frequency analysis and feature fusion  
- `src/validation_model.ipynb` → Model evaluation and testing

### 🧠 Trained Model
- Trained model file: `models/deepfake_model.h5`  
- [Download Link](https://drive.google.com/your_model_link)

