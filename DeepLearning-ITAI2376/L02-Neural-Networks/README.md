# L02 — Neural Network Foundations

## Project Overview

In this lab, I built a strong foundation in neural networks by implementing core concepts from scratch and then reproducing them using modern frameworks. I wanted to understand what happens *inside* a model before relying on high-level APIs.

## Problem Statement

I explored how feedforward neural networks learn representations and how model choices (architecture, regularization, hyperparameters) affect performance on image classification tasks.

## My Approach

I worked through three stages:
1. Implemented neural network fundamentals conceptually and numerically.
2. Built training pipelines in **PyTorch** and **TensorFlow/Keras**.
3. Compared performance trends and overfitting behavior while tuning parameters.

## Datasets

- **Fashion-MNIST** (primary lightweight dataset)
- **CIFAR-10** (advanced option)
- References to MNIST setup/variants in notebook workflow

## Technologies Used

- Python
- NumPy
- PyTorch
- TensorFlow / Keras
- Matplotlib, Seaborn
- scikit-learn

## Key Results

From the captured notebook runs:
- Validation accuracy improved steadily from about **85.12%** to around **88.93%** in one run.
- Best observed training output reached approximately **91.88% accuracy**.
- Framework-based implementations converged faster than manual implementations while preserving the same conceptual pipeline.

## Visual Results

See `results/`:
- `fashion_mnist_sample_grid.png`
- `visualization_inventory.md`

## What I Learned

- Building from scratch made backpropagation and gradient flow much more intuitive.
- Small hyperparameter changes (learning rate, dropout, epochs) can shift validation performance significantly.
- PyTorch and TensorFlow differ in style, but both map cleanly to the same core learning principles.

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook Neural_Networks_Foundations.ipynb
```

Or open the notebook in Google Colab and run all cells in order.
