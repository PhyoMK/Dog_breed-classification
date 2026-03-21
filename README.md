# 🐶 Dog Breed Classification (120 Breeds)

## 📑 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Model Development](#model-development)
- [Deployment](#deployment)
- [Future Improvements](#future-improvements)

---

## 📌 Overview
The **Dog Breed Classification Model** is a deep learning project designed to accurately identify dog breeds from input images.

This project uses a pre-trained Convolutional Neural Network (CNN) to classify images into **120 different dog breeds**. The goal is to build a robust and scalable model that performs well on unseen data.

---

## 📂 Dataset
Dataset source:  
https://www.kaggle.com/datasets/jessicali9530/stanford-dogs-dataset  

### 🔹 Data Preparation
- Downloaded and stored in a local `data/` directory  
- Resized all images to match the model input size  
- Split dataset into:
  - **Training set**: 80%  
  - **Validation set**: 10%  
  - **Test set**: 10%  

### 📁 Folder Structure
data/
├── train/
├── val/
└── test/

---

## 🧠 Model Development

### 🔹 Data Preprocessing
- Image resizing  
- Normalization  
- Dataset split (80/10/10)  

---

### 🔹 Model Architecture
- Pre-trained CNN (e.g., Xception / ResNet / MobileNet)  
- Global Average Pooling layer  
- Dense layer with ReLU activation  
- Output layer with **120 classes**  

---

### 🔹 Training Process
- Optimizer: **Adam**  
- Loss Function: **Categorical Crossentropy**  
- Trained using training set and validated on validation set  
- Hyperparameters tuned for better performance  

---

### 🔹 Model Saving
- Best model saved based on validation performance  

---

### 🔹 Model Evaluation
- Evaluated using test dataset  
- Accuracy calculated  
- Tested with single image predictions  

---

## 🚀 Deployment

### 🔹 Local Server
- Built using **Flask**  
- Features:
  - Upload image  
  - Predict dog breed  
  - Display prediction results  

---

### 🔹 Cloud Access
- Exposed locally hosted server using **Cloudflare Tunnel (`cloudflared`)**  
- Enabled remote access without port forwarding  

---

## 💡 Future Improvements
- Data augmentation for better accuracy  
- Use lightweight models for edge devices (TinyML / IoT)  
- Real-time camera prediction  
- Cloud deployment (AWS / GCP / Azure)  

---

## 👨‍💻 Author
**Phyo Min Khant**  
Electrical Engineering (Mechatronics) Student  
