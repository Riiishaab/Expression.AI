
📘 FER2013 Dataset Overview

The Facial Expression Recognition 2013 (FER2013) dataset is a widely used benchmark in the field of facial expression recognition. Key characteristics include:
 -> Image Details: Consists of 48×48 pixel grayscale images of human faces.​
 -> Dataset Size: Contains a total of 35,887 images, divided into:​
 -> Training set: 28,709 images​
 -> Test set: 3,589 images​

Emotion Categories: Each image is labeled with one of seven emotions:​

-> Angry​
-> Disgust​
-> Fear​
-> Happy​
-> Sad​
-> Surprise​
-> Papers with Code
-> Neutral​


Challenges:

-> Class Imbalance: Some emotions, like 'Disgust', have significantly fewer samples compared to others, leading to class imbalance issues.​
-> Variability: Images exhibit variations in lighting, occlusions, and facial orientations, making recognition tasks more challenging.​
-> Label Noise: There are instances of mislabeling within the dataset, which can affect model training and evaluation.​


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

📊 Literature Review: Model Accuracies on FER2013

Over the years, numerous models have been developed and tested on the FER2013 dataset. Below are five notable models along with their reported accuracies:​

1 -> VGGNet-Based Model:
           Accuracy: 73.28%​
           Details: Achieved by fine-tuning a VGGNet architecture with optimized hyperparameters and learning rate schedulers.​

2 -> Ensemble of 7 Models by Khanzada et al.
           Accuracy: 75.8%​
           Details: Combined predictions from seven different models to enhance overall accuracy.​

3 -> EmoXNet Ensemble Model:
           Accuracy: 85.07%​
           Details: An ensemble learning technique that integrates multiple architectural representations for robust facial expression recognition.​

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

📊 Expression.AI Model Performance Overview

✅ After training for approximately 130 epochs, our custom hybrid model achieved a test accuracy of 69.32%.
⚖️ This accuracy reflects a well-balanced trade-off between model size and performance, making it ideal for mobile deployment.
📦 The entire mobile application, including the deep learning model, OpenCV libraries, and UI assets, is only 595 MB, which is significantly lightweight for modern smartphones.
🚀 Despite the compact size, the model delivers reliable real-time predictions on device, showcasing the effectiveness of the architecture.

🔬 Future work will focus on experimenting with:
      -> More efficient architectures like blocks of MobileNetV3, EfficientNet-Lite, or quantized models.
      -> Knowledge distillation or pruning techniques to reduce model size further while improving generalization.
      -> Integration of transfer learning for better initialization and faster convergence.
