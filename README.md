# 🧠 Brain Tumor Detection using ResNet50 (Transfer Learning)

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-DeepLearning-red)
![Model](https://img.shields.io/badge/Model-ResNet50-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Accuracy](https://img.shields.io/badge/Accuracy-78%25-yellow)

---

## 📌 Overview
This project presents a deep learning-based solution for detecting brain tumors from MRI images using transfer learning with a pretrained ResNet50 model. The system classifies images into four categories:
- Glioma  
- Meningioma  
- Pituitary Tumor  
- No Tumor  

---

## 🧠 Model Architecture
- Pretrained ResNet50 (ImageNet weights)  
- Frozen initial layers  
- Fine-tuned last convolutional block (layer4)  
- Custom fully connected classification layer  

---

## ⚙️ Tech Stack
- Python  
- PyTorch  
- TensorFlow (for initial testing)  
- NumPy  
- Matplotlib  
- PIL  

---

## 📂 Dataset Structure

```
Training/
    glioma/
    meningioma/
    notumor/
    pituitary/

Testing/
    glioma/
    meningioma/
    notumor/
    pituitary/
```

---

## 🔄 Data Preprocessing
- Resize images to 256 → Crop to 224  
- Random Horizontal Flip  
- Random Rotation & Affine Transformations  
- Normalization using ImageNet statistics  

---

## 🏋️ Training Details
- Epochs: 40  
- Batch Size: 32  
- Optimizer: Adam (lr = 0.0001)  
- Loss Function: CrossEntropyLoss  
- Scheduler: StepLR  

---

## 📊 Results
✔️ Achieves strong validation accuracy  
✔️ Generalizes well on unseen MRI images  

---

## 🔍 Prediction Example
You can test the model on a single MRI image:

Predicted Class: meningioma

![Prediction](https://github.com/user-attachments/assets/df65df4d-a033-490c-810d-d62c877d9b85)

---

## 💡 Future Improvements
- Increase dataset size for better accuracy  
- Use advanced models (EfficientNet, DenseNet)  
- Add Grad-CAM visualization  
- Deploy as full-stack web app (React + API)   

---

## ⚠️ Disclaimer
This project is for educational purposes only and should not be used for medical diagnosis.

---

## ⭐ Support
If you like this project:
- ⭐ Star the repo  
- 🍴 Fork it  
- 🛠️ Contribute  

---

## 👨‍💻 Author
Kashif Ullah Khan
