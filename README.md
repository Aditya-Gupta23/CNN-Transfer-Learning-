# Transfer Learning for Fashion MNIST Classification using VGG16

## Overview

This project demonstrates the use of **Transfer Learning** with the pretrained **VGG16** Convolutional Neural Network (CNN) in PyTorch for image classification on the Fashion MNIST dataset.

Instead of training a deep CNN from scratch, a pretrained VGG16 model is leveraged to extract meaningful visual features, significantly reducing training time and improving performance. Since Fashion MNIST contains grayscale images of size 28×28, the images are preprocessed and resized to match the input requirements of VGG16.

## Dataset

Fashion MNIST Dataset:

https://www.kaggle.com/datasets/zalando-research/fashionmnist

The dataset contains 70,000 grayscale images belonging to 10 fashion categories:

- T-shirt/Top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle Boot

## Project Structure

```text
.
├── Transfer_Learning_CNN_PyTorch.ipynb
├── fashion-mnist_train.csv
├── fashion-mnist_test.csv
└── README.md
```

## Model Architecture

The project uses the pretrained **VGG16** model available in Torchvision.

### Why VGG16?

- Pretrained on the ImageNet dataset containing over 1 million images.
- Learns rich visual representations that can be transferred to new tasks.
- Simple and effective CNN architecture.
- Widely used as a baseline for transfer learning experiments.

### Workflow

```text
Fashion MNIST Images
          ↓
Image Preprocessing
          ↓
Resize to VGG16 Input Size
          ↓
Pretrained VGG16
          ↓
Modified Classification Head
          ↓
Fashion Category Prediction
```

## Features

- Data preprocessing and normalization
- Transfer learning using VGG16
- Custom PyTorch Dataset and DataLoader
- Training and validation pipeline
- Performance evaluation on unseen data
- Visualization of sample predictions

## Technologies Used

- Python
- PyTorch
- Torchvision
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Installation

```bash
pip install torch torchvision pandas numpy matplotlib scikit-learn
```

## Running the Project

1. Download the Fashion MNIST dataset from Kaggle.
2. Place the dataset files in the project directory.
3. Launch Jupyter Notebook:

```bash
jupyter notebook Transfer_Learning_CNN_PyTorch.ipynb
```

4. Run all notebook cells sequentially to:
   - Load and preprocess data
   - Initialize the pretrained VGG16 model
   - Train the classifier
   - Evaluate model performance

## Learning Objectives

This project helps in understanding:

- Convolutional Neural Networks (CNNs)
- Transfer Learning
- Feature Extraction using pretrained models
- VGG16 architecture
- Image preprocessing in PyTorch
- Building end-to-end image classification pipelines


