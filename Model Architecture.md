
**🔗 [Download APK](https://github.com/Riiishaab/Expression.AI/releases/download/v1.0/ExpressionAI.apk)**
 

---

## 🧱 ResEfficientCNN Architecture (Overview)

```
🚀 Deep Hybrid CNN Architecture
            ⬇️
📥 Input Layer (224x224x1)
            ⬇️
🧠 Conv2D(64, 7x7, stride=2) + BatchNorm + ReLU
            ⬇️
🌀 MaxPooling2D(3x3, stride=2, padding='same')
            ⬇️
🔁 Residual Block (filters=64, downsample=True)
            ⬇️
🔗 Inception Block (64, 32→64, 16→32, pool=32)
            ⬇️
🔁 Residual Block (filters=128, downsample=True)
            ⬇️
🔗 Inception Block (128, 64→128, 32→64, pool=64)
            ⬇️
🔁 Residual Block (filters=128, downsample=True)
            ⬇️
🔗 Inception Block (128, 64→128, 32→64, pool=64)
            ⬇️
🔁 Residual Block (filters=256, downsample=True)
            ⬇️
🔗 Inception Block (256, 128→256, 64→128, pool=128)
            ⬇️
🔁 Residual Block (filters=256, downsample=True)
            ⬇️
🔗 Inception Block (256, 128→256, 64→128, pool=128)
            ⬇️
🔽 Global Average Pooling 2D
            ⬇️
🧱 Dense(512) → BatchNorm → Dropout(0.5)
            ⬇️
🧱 Dense(256) → BatchNorm → Dropout(0.5)
            ⬇️
🎯 Dense(7, activation='softmax')
            ⬇️
📤 Output: 7-class prediction
```

---

## 🔎 Layer-wise Breakdown

### 📥 Input Layer
- **Shape**: (224, 224, 1)
- Grayscale facial image resized to 224x224 pixels

### 🧠 Initial Convolution
- **Conv2D(64, 7x7, stride=2)**: Extracts high-level spatial features
- **BatchNormalization**: Stabilizes and accelerates training
- **ReLU Activation**: Introduces non-linearity

### 🌀 MaxPooling
- **MaxPooling2D(3x3, stride=2)**: Downsamples spatial dimensions

### 🔁 Residual Block
- Two Conv2D layers + BatchNorm + ReLU
- Identity or projection shortcut
- Helps in deeper network training by mitigating vanishing gradients

### 🔗 Inception Block
- **1x1 Conv**: Dimensionality reduction
- **1x1 → 3x3 Conv**: Medium-range patterns
- **1x1 → 5x5 Conv**: Wide contextual capture
- **3x3 MaxPool → 1x1 Conv**: Spatial info preservation

### 📉 Global Average Pooling
- Reduces each feature map to a single value
- Less prone to overfitting than flattening

### 🧱 Dense Layers
- **Dense(512)** → **BatchNorm** → **Dropout(0.5)**
- **Dense(256)** → **BatchNorm** → **Dropout(0.5)**
- Regularization and feature refinement

### 🎯 Output Layer
- **Dense(7, activation='softmax')**
- Outputs probability scores for each emotion category

---


> We hope you enjoy using **Expression.AI** as much as we enjoyed building it!

