# 🛡️ Smart Surveillance: Real-Time Face Mask Detection Using MobileNetV2

This project presents a **real-time face mask detection system** powered by deep learning and computer vision.  
By leveraging the lightweight and efficient **MobileNetV2** architecture, the system accurately identifies whether individuals are wearing face masks using live webcam or video stream input.

---

## 🚀 Features

- 🎥 **Live face detection** using OpenCV’s Haar Cascade classifiers  
- 🤖 **Mask classification** via a fine-tuned **MobileNetV2** network  
- 📊 **High Accuracy:**  
  - **Accuracy:** 98.32%  
  - **F1-Score:** 0.98 on a test set of 1908 samples  
- 🖼️ **Visual output** with color-coded bounding boxes:  
  - 🟩 Green: With Mask  
  - 🟥 Red: Without Mask  

---

## 🤖 Model Architecture

- **Base Model:** Pre-trained **MobileNetV2** (used as a frozen feature extractor)  
- **Custom Head:** Fully-connected layers with **ReLU**, **Dropout**, and **Softmax** activation  
- **Training Enhancements:**  
  - Data Augmentation (rotation, flip, zoom)  
  - **Loss Function:** Categorical Cross-Entropy  
  - **Optimizer:** Adam (`lr=0.001`)  
  - **Callbacks:** EarlyStopping, Learning Rate Scheduler  

---

## 📊 Dataset

- [Face Mask Detection Dataset – Kaggle](https://www.kaggle.com/datasets/shiekhburhan/face-mask-dataset?select=FMD_DATASET)  
- Contains labeled images of faces **with** and **without** masks, in varied real-world settings

---


