# denseNet-pneumonia
Chest X-ray pneumonia classification using DenseNet121 and deep learning


### Why DenseNet121?

DenseNet introduces dense connectivity —> each layer receives inputs from all previous layers.
Encourages feature reuse
Reduces number of parameters compared to ResNet
Captures fine-grained medical features effectively
Proven strong performance on image classification tasks


### Methodology

Preprocessing
Image resizing to 224×224
Data augmentation (rotation, flip, zoom, shift)
Model Training
Base model: DenseNet121 with imagenet weights
Frozen initial layers -> trained top layers
Fine-tuned deeper layers (epochs 6–10)
Optimizer: Adam with learning rate scheduling
Evaluation Metrics
Accuracy
Precision, Recall, F1-score
Confusion Matrix





### The trained DenseNet121 model (~38 MB) can be downloaded from here:  
[Download densenet_pneumonia.keras](https://drive.google.com/file/d/1YEGf4MAec4UnT4Yp4G1Uz7VBCl4WG1NW/view?usp=sharing)

