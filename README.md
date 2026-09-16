# 🛡️ Smart Surveillance: Real-Time Face Mask Detection Using MobileNetV2

This project implements a **real-time face mask detection system** using deep learning and computer vision.  
Leveraging the **MobileNetV2** architecture, the system determines whether a person is wearing a face mask or not using live video input from a webcam or video stream.

---

##  Features
- **Real-time face detection** using Haar Cascade classifiers (OpenCV)
- **Mask classification** using fine-tuned MobileNetV2
- **Performance:** Accuracy: **98.32%**, F1-Score: **0.98** on 1908 test samples
- **Output rendering** with color-coded bounding boxes  (Green = Mask, Red = No Mask)

---

##  Model Overview
- **Backbone:** Pre-trained **MobileNetV2** used as a feature extractor
- **Classification Head:** Custom dense layers with **Dropout** and **ReLU** activation
- **Training Data:** Augmented dataset containing real-world and synthetic face images
- **Loss Function:** Categorical Cross-Entropy  
-  **Optimizer:** Adam (lr = 0.001), with Early Stopping and LR Scheduler

---

##  Dataset Used
- [Face Mask Detection Dataset – Kaggle](https://www.kaggle.com/datasets/shiekhburhan/face-mask-dataset?select=FMD_DATASET)

---
