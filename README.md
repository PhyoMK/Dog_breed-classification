🐶 Dog Breed Classification (120 Breeds)
📑 Table of Contents
Overview
Dataset
Model Development
Deployment
📌 Overview

The Dog Breed Classification Model is an image classification project designed to accurately identify dog breeds from input images.

This project leverages deep learning techniques and uses a pre-trained Convolutional Neural Network (CNN) architecture to classify images into 120 different dog breeds. The goal is to build a robust and scalable model that can generalize well to unseen images.

📂 Dataset

Dataset used:
👉 https://www.kaggle.com/datasets/jessicali9530/stanford-dogs-dataset

🔹 Data Preparation
The dataset was downloaded and stored in a local data/ directory.
All images were resized to match the model’s required input size.
The dataset was split into three subsets:
Training set: 80%
Validation set: 10%
Test set: 10%

The images were organized into separate folders:

data/
  ├── train/
  ├── val/
  └── test/
🧠 Model Development
🔹 Data Preprocessing
Images were resized to a fixed input size suitable for the model.
Data was normalized using standard preprocessing techniques.
The dataset was split into training, validation, and testing sets (80/10/10).
🔹 Model Architecture
A pre-trained CNN model (e.g., Xception / ResNet / MobileNet) was used as the base model.
Feature extraction layers were followed by:
Global Average Pooling layer
Dense (fully connected) layer
Output layer with 120 classes
🔹 Training Process
Optimizer: Adam
Loss Function: Categorical Crossentropy
The model was trained on the training dataset and validated using the validation dataset.
Hyperparameters such as learning rate and batch size were tuned to improve performance.
🔹 Model Saving
The best model was saved during training using validation performance (e.g., lowest validation loss or highest validation accuracy).
🔹 Model Evaluation
The final model was evaluated using the test dataset.
Accuracy was calculated to measure performance.
Additionally, the model was tested using individual images to verify real-world usability.
🚀 Deployment

The trained model was deployed locally using Flask as a web server.

🔹 Features:
Upload an image via a web interface
Predict dog breed
Display top predictions
🔹 Cloud Access:

The local Flask server was exposed to the internet using Cloudflare Tunnel (cloudflared), allowing remote access without port forwarding.

💡 Future Improvements
Improve model accuracy with data augmentation
Use lightweight models for edge deployment (TinyML / IoT)
Add real-time camera prediction
Deploy to cloud platforms
