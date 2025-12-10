# 🩺 Breast Cancer Detection Web App  

A deep-learning powered web application built using **Flask** that predicts whether a breast tumor is **Benign** or **Malignant** from an uploaded image using a trained CNN model.

---

## 🚀 Project Overview
This project uses a **Convolutional Neural Network (CNN)** trained on breast cancer histopathology images.  
Users can upload an image, and the app will classify it as:

- **Benign**
- **Malignant**

The application preprocesses the uploaded image, passes it into the trained `.h5` model, and returns both the **prediction** and **confidence score**.

---
## 📂 Download Links

- **Model (on Hugging Face):** https://huggingface.co/BhMunira/benign-malignant-classifier  
- **Dataset (on Google Drive):** https://drive.google.com/drive/folders/1JEr-1rJViRLwX2q-su6uQI_0WNoySkYL
  
----

## 🧠 How It Works
1. User uploads an image.
2. Image is saved inside `static/uploads/`.
3. CNN model (`breast_cancer_model.h5`) loads automatically when the server s4. Image is:
   - resized to **150×150**
   - normalized
   - expanded to batch shape  
5. Model prediction:
   - Output > 0.5 → **Malignant**
   - Output ≤ 0.5 → **Benign**

---

## 🗂️ Tech Stack

### **Backend**
- Python  
- Flask  
- TensorFlow / Keras  
- OpenCV  

### **Frontend**
- HTML  
- CSS  
- Jinja Templates  

---

**## 📁 Project Structure
├── app.py
├── breast_cancer_model.h5
├── templates/
│ └── index.html
├── static/
│ └── uploads/
└── README.md**
