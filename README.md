# Cat vs Dog vs Panda Image Classification using Transfer Learning

## Name: Joel John Jobinse
## Register No: 212223240062

## Project Overview

This project performs image classification using Transfer Learning in PyTorch to classify images into three categories:

- Cat
- Dog
- Panda

The model uses a pre-trained ResNet18 network from TorchVision and fine-tunes the classifier layers for multi-class image classification.

---

## Dataset

Dataset used:

Cats Dogs Pandas Images Dataset

Kaggle Dataset:

https://www.kaggle.com/datasets/gpiosenka/cats-dogs-pandas-images

Dataset structure:

data/

│── cat/

│── dog/

└── panda/

Images are resized to 224 × 224 and normalized using ImageNet statistics.

---

## Features

- Transfer Learning using ResNet18
- CUDA GPU support
- Data augmentation
- Training and validation split
- Best model checkpoint saving
- Confusion matrix visualization
- Image prediction function
- Reproducible results using random seeds

---

## CUDA Verification

Run before training:

```python
import torch

print("CUDA available:", torch.cuda.is_available())

device = torch.device(
    "cuda"
    if torch.cuda.is_available()
    else "cpu"
)

print(device)
```

## Output:
### Dataset:
<img width="812" height="748" alt="image" src="https://github.com/user-attachments/assets/d7d9f4e7-7a18-4e6b-b206-845356ae801b" />

### ResNet:
<img width="967" height="737" alt="image" src="https://github.com/user-attachments/assets/654aba6b-6831-4a2d-b876-ec23fadef638" />

### Epochs:
<img width="455" height="330" alt="image" src="https://github.com/user-attachments/assets/0fcac2c1-8bc4-4493-98f8-2c3ad37af39f" />

### Accuracy:
<img width="211" height="32" alt="image" src="https://github.com/user-attachments/assets/84be47ad-38ff-4547-b039-67c065ce706e" />

### Confusion Matrix:
<img width="923" height="713" alt="image" src="https://github.com/user-attachments/assets/4be6e6ca-2a02-478d-bf85-e218c8318413" />
