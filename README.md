# Plant Disease Detection using Vision Transformer

## Overview
This repository contains an implementation of a Vision Transformer (ViT) model for automated plant disease detection. The model achieves high accuracy in identifying various plant diseases using the PlantVillage dataset, demonstrating the effectiveness of transformer-based architectures in agricultural applications.

## Model Performance
- **Test Accuracy**: 91.38%

This impressive accuracy demonstrates the model's robust performance in identifying plant diseases across different classes and plant species.

## Model Architecture
The implementation uses a Vision Transformer (ViT) architecture, which has shown remarkable performance in computer vision tasks. Key features include:

- Patch Embedding layer for converting images into sequences of patches
- Multiple transformer encoder blocks
- Multi-head self-attention mechanisms
- Position embeddings
- MLP head for classification
- Layer normalization and dropout for regularization

## Dataset
This project uses the PlantVillage dataset, a comprehensive collection of plant disease images.

### Dataset Characteristics:
- **Source**: PlantVillage Dataset
- **Number of Classes**: 15 different classes
- **Plants Covered**: 3 plant species (Tomato, Potato, Pepper Bell)

### Classes by Plant Type:

#### Tomato (9 classes):
1. Tomato Healthy
2. Tomato Leaf Mold
3. Tomato Yellow Leaf Curl Virus
4. Tomato Bacterial Spot
5. Tomato Septoria Leaf Spot
6. Tomato Spider Mites (Two-spotted Spider Mite)
7. Tomato Early Blight
8. Tomato Target Spot
9. Tomato Late Blight
10. Tomato Mosaic Virus

#### Potato (3 classes):
1. Potato Healthy
2. Potato Late Blight
3. Potato Early Blight

#### Pepper Bell (2 classes):
1. Pepper Bell Bacterial Spot
2. Pepper Bell Healthy

### Preprocessing Steps:
1. Image resizing to 224×224 pixels
2. Normalization using ImageNet statistics
3. Data augmentation techniques

### Data Augmentation:
- Random horizontal flip
- Random rotation (±20 degrees)
- Random brightness adjustment
- Random contrast adjustment
- Random crop and resize
- ColorJitter

## Requirements
```
python>=3.8
torch>=1.9.0
torchvision>=0.10.0
timm>=0.5.4  # for ViT implementations
pandas
numpy
Pillow
scikit-learn
matplotlib
albumentations
```

## Installation
```
git clone https://github.com/HarshGosula/Plant_Disease_Detection_using_Vision_Transformers.git

```
