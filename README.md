#  AI-Based Pneumonia Diagnosis System

An **AI-powered medical diagnosis system** that detects **Pneumonia from chest X-ray images** using **Deep Learning and Transfer Learning**.  
The trained model is deployed using **Gradio**, allowing users to upload X-ray images and receive instant predictions.

---

## 📌 Project Overview

Pneumonia is a serious lung infection that requires early detection.  
This project uses a **pretrained ResNet50 model** to classify chest X-ray images into:

- **Normal**
- **Pneumonia**

The system is designed as an **end-to-end machine learning project**, covering training, evaluation, and deployment.

---

## 🧠 Technologies Used

- Python  
- TensorFlow / Keras  
- ResNet50 (Transfer Learning)  
- NumPy  
- Pillow (PIL)  
- Scikit-learn  
- Gradio  
- Matplotlib  

---


## 🗂 Dataset

- **PneumoniaMNIST**
- **Chest X-Ray Images (Pneumonia) – Kaggle**

Classes:
- `0` → Normal  
- `1` → Pneumonia  

Images are resized to **224×224** and converted to **RGB** before training.

---

## ⚙️ Model Architecture

- **Base Model:** ResNet50 (ImageNet pretrained)
- **Transfer Learning:** Yes (base layers frozen)
- **Custom Layers:**
  - Global Average Pooling
  - Dense (ReLU)
  - Dense (Softmax – 2 classes)

**Optimizer:** Adam  
**Loss Function:** Sparse Categorical Crossentropy  
**Metric:** Accuracy  

---
## 📊 Results

Good classification accuracy on validation data

Effective use of transfer learning

Real-time prediction via web interface

---

⚠️ Disclaimer

It should not be used for real medical diagnosis.
