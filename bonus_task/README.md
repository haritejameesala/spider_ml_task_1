# Bonus Task - Fashion MNIST Autoencoder

## Overview

This project implements an Autoencoder using PyTorch on the Fashion-MNIST dataset. The model learns a compact latent representation of clothing images and reconstructs the original images from the compressed encoding.

## Dataset

Fashion-MNIST is a collection of 28×28 grayscale images belonging to 10 clothing categories.

Dataset:
https://www.kaggle.com/datasets/zalando-research/fashionmnist

## Model Architecture

### Encoder
- Input: 784
- Linear(784 → 128) + ReLU
- Linear(128 → 64) + ReLU
- Linear(64 → 32) + ReLU

### Latent Space
- Dimension: 32

### Decoder
- Linear(32 → 64) + ReLU
- Linear(64 → 128) + ReLU
- Linear(128 → 784)
- Sigmoid Activation

## Objective

The Autoencoder is trained to:

- Compress input images into a 32-dimensional latent representation.
- Reconstruct the original image from the compressed representation.
- Minimize reconstruction error between the input and reconstructed image.

## Training Details

- Framework: PyTorch
- Optimizer: Adam
- Loss Function: Mean Squared Error (MSE)
- Batch Size: 64
- Epochs: 20
- Train/Validation Split: 80/20

## Results

The project includes:

- Training Loss Curve
- Validation Loss Curve
- Original vs Reconstructed Image Comparisons

The decreasing reconstruction loss demonstrates that the Autoencoder successfully learns meaningful compressed representations of Fashion-MNIST images.

## Repository Contents

- `code/` – Autoencoder implementation notebook
- `results/` – Loss plots and reconstruction outputs

## Author

Hari Teja  
B.Tech CSE, NIT Trichy