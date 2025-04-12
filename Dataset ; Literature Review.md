📘 FER2013 Dataset Overview
The Facial Expression Recognition 2013 (FER2013) dataset is a widely used benchmark for training and evaluating facial emotion classification models.

📂 Key Characteristics:

Image Details: 48×48 pixel grayscale images of human faces

Total Images: 35,887

Training Set: 28,709 images

Test Set: 3,589 images

🧠 Emotion Categories:

😠 Angry

🤢 Disgust

😨 Fear

😄 Happy

😢 Sad

😲 Surprise

😐 Neutral

⚠️ Challenges:

Class Imbalance: Some emotions like Disgust have significantly fewer examples

Variability: Faces differ in lighting, orientation, and occlusions

Label Noise: Occasional mislabeling in training/testing samples

📊 Literature Review: Model Accuracies on FER2013
Several advanced models have been developed to push the boundaries of facial expression recognition on FER2013. Below are some notable results:

🧪 Model	⚙️ Description	🎯 Accuracy
VGGNet-Based	Fine-tuned VGGNet with hyperparameter tuning and LR scheduling	73.28%
Khanzada et al. (Ensemble of 7)	Combined predictions of 7 deep models	75.80%
EmoXNet Ensemble	Multi-architecture ensemble method	85.07%
📱 Expression.AI Model Performance
Our hybrid deep learning architecture was designed with mobile deployment in mind — achieving a strong balance of accuracy, efficiency, and real-time performance.

📌 Highlights:

✅ Final Accuracy: 69.32% after ~130 epochs of training

⚖️ Size vs. Performance: Optimized for deployment on Android devices

📦 APK Size: Entire app including model, assets & OpenCV is only 595 MB

🚀 Deployment: Runs real-time inference with smooth UI & fast predictions

🔬 Future Work
We aim to further enhance accuracy and reduce model complexity in upcoming versions:

🔧 Explore lightweight architectures like MobileNetV3, EfficientNet-Lite

🧠 Apply Knowledge Distillation and Pruning to compress the model

♻️ Integrate transfer learning for better convergence and generalization
