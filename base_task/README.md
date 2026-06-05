# Spider ML Task 1 – Fashion-MNIST Classification

This repository contains my submission for **Spider R&D SPML Task 1**. The project implements the neural network architecture provided in the problem statement using **PyTorch** and trains it on the **Fashion-MNIST** dataset.

## Overview

The objective of this task is to build and train a neural network for Fashion-MNIST image classification while implementing a complete deep learning pipeline, including training, evaluation, visualization, model saving, and prediction generation.

## Model Architecture

The implemented architecture follows the structure specified in the task:

- Input Layer: 784 neurons (28×28 flattened image)
- Hidden Layer: 16 neurons
- Branch 1: 16 → 8 → 8 (with skip connection)
- Branch 2: 16 → 12 → 8
- Concatenation of both branches
- Output Layer: 10 neurons (Fashion-MNIST classes)

## Dataset

**Fashion-MNIST Dataset**

Source:  
https://www.kaggle.com/datasets/zalando-research/fashionmnist

Files used:

- `fashion-mnist_train.csv`
- `fashion-mnist_test.csv`

The dataset files are not included in this repository due to their large size and can be downloaded from the above source.

## Technologies Used

- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Pickle

## Training Pipeline

- Data loading and preprocessing
- Model implementation using PyTorch
- Forward and backward propagation
- Training and validation loops
- Accuracy and loss tracking
- Model checkpoint saving
- Prediction generation
- Performance visualization

## Results

The notebook includes:

- Training Loss vs Epochs
- Validation Loss vs Epochs
- Training Accuracy vs Epochs
- Validation Accuracy vs Epochs

These metrics are plotted using Matplotlib for performance analysis.

## Files Included

- `Fashion_MNIST.ipynb` — Main notebook
- `best_model.pkl` — Saved model weights
- `submission.csv` — Model predictions
- Accuracy/Loss plots

## How to Run

1. Clone the repository

```bash
git clone https://github.com/haritejameesala/spider_ml_task_1.git
```

2. Install dependencies

```bash
pip install torch torchvision numpy pandas matplotlib
```

3. Open and run the notebook

```bash
jupyter notebook Fashion_MNIST.ipynb
```

## Author

**Hari Teja Meesala**  
B.Tech CSE, National Institute of Technology Tiruchirappalli
