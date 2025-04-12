# 🤖 Expression.AI - Facial Emotion Recognition Android App

**🔗 [Download APK](https://your-apk-link-here.com)**

---

## 📘 FER2013 Dataset Overview

The **Facial Expression Recognition 2013 (FER2013)** dataset is a widely used benchmark in facial expression recognition.

### 🔍 Dataset Highlights:
- 📐 **Image Size**: 48×48 pixel grayscale facial images  
- 🗃️ **Total Samples**: 35,887 images  
  - **Training Set**: 28,709 images  
  - **Test Set**: 3,589 images  
- 😄 **Emotion Labels** (7 classes):
  - Angry  
  - Disgust  
  - Fear  
  - Happy  
  - Sad  
  - Surprise  
  - Neutral  

### ⚠️ Challenges:
- ⚖️ **Class Imbalance**: Some emotions (e.g., *Disgust*) have very few samples  
- 🌩️ **Variability**: Faces differ in lighting, occlusions, and pose  
- 🏷️ **Label Noise**: Occasional mislabeling affects training quality  

---

## 📊 Literature Review: Model Accuracies on FER2013

Here are some top models and their performance on the FER2013 dataset:

1. **VGGNet-Based Model**  
   - 📈 Accuracy: **73.28%**  
   - 🛠️ Details: Fine-tuned VGG architecture with optimized learning strategies  

2. **Khanzada et al. (Ensemble of 7 Models)**  
   - 📈 Accuracy: **75.8%**  
   - 🤖 Details: Combined predictions from 7 individual networks  

3. **EmoXNet Ensemble**  
   - 📈 Accuracy: **85.07%**  
   - 🔬 Details: Multiple architectural branches merged for final prediction  

---

## 📊 Expression.AI Model Performance Overview

- ✅ After training for around **130 epochs**, our **custom hybrid model** reached a **test accuracy of 69.32%**
- ⚖️ This accuracy reflects a balanced trade-off between **model size** and **performance**
- 📦 The **entire mobile app package** (including model, OpenCV, and UI) is **just 595 MB**
- 🚀 Runs **smoothly in real-time** on Android, showing efficient architecture deployment

---

## ⚙️ Tech Stack

- 🧠 **Model Type**: Hybrid Residual + Inception CNN  
- 📊 **Framework**: TensorFlow/Keras  
- 📱 **Deployment**: Android Studio (Jetpack Compose + PyTorch Lite)  
- 🎨 **Libraries**: OpenCV, CameraX

---

## 🔬 Future Work

We plan to improve the model further through:
- 📱 Lightweight backbones like **MobileNetV3**, **EfficientNet-Lite**, or **quantized CNNs**
- 🧠 **Knowledge distillation** or **pruning** to reduce size and inference latency  
- 🧬 **Transfer learning** to enable faster convergence and better initialization  

---

## 🎉 Why Expression.AI?

- 🤳 **Fun**: Use it with friends, family, and colleagues
- ⚡ **Fast**: Real-time inference on-device
- 🧠 **Smart**: Deep learning on mobile

---

> We hope you enjoy using **Expression.AI** as much as we enjoyed building it!

