# denseNet-pneumonia
Chest X-ray pneumonia classification using DenseNet121 and deep learning



🩺 Pneumonia Detection from Chest X-Rays using DenseNet121

📌 Overview

Early detection of Pneumonia from chest X-rays is crucial for saving lives.
In this project, I built and fine-tuned a DenseNet121-based CNN model to classify chest X-rays as:
Normal
Pneumonia
The model achieved strong performance while keeping the architecture efficient.


⚙️ Dataset
Source: Kaggle Chest X-Ray Pneumonia Dataset

Total images: ~5,800

Train: 5,216

Validation: 16

Test: 624


🧠 Why DenseNet121?

DenseNet introduces dense connectivity — each layer receives inputs from all previous layers.
✅ Encourages feature reuse
✅ Reduces number of parameters compared to ResNet
✅ Captures fine-grained medical features effectively
✅ Proven strong performance on image classification tasks


🔧 Methodology

Preprocessing
Image resizing to 224×224
Data augmentation (rotation, flip, zoom, shift)
Model Training
Base model: DenseNet121 with imagenet weights
Frozen initial layers → trained top layers
Fine-tuned deeper layers (epochs 6–10)
Optimizer: Adam with learning rate scheduling
Evaluation Metrics
Accuracy
Precision, Recall, F1-score
Confusion Matrix


📊 Results

Metric	Value

Training Accuracy	97.1%

Validation Accuracy	87.5%

Test Accuracy	86.7%

F1-score	90.2%



🔮 Future Improvements
Train longer (30–50 epochs) with early stopping
Try EfficientNet for better efficiency
Apply Grad-CAM for explainable AI (visualizing heatmaps)
Use larger, more diverse datasets

The trained DenseNet121 model (~38 MB) can be downloaded here:  
[Download densenet_pneumonia.keras](https://drive.google.com/file/d/1YEGf4MAec4UnT4Yp4G1Uz7VBCl4WG1NW/view?usp=sharing)
