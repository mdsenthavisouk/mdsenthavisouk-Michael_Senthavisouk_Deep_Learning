# L03 — CNN: Puppy vs Bagel Classification

## Project Overview

In this lab, I trained convolutional neural networks to solve a fun but non-trivial binary image classification problem: distinguishing **puppies** from **bagels**.

## Problem Statement

The visual similarity between curled-up puppies and bagels makes this a useful challenge for understanding how CNNs extract discriminative visual features.

## My Approach

I built and evaluated:
1. A custom CNN baseline in TensorFlow/Keras
2. Data preprocessing and augmentation pipeline
3. Transfer learning experiments with pretrained backbones
4. Evaluation with validation accuracy and test behavior checks

## Dataset

- **Puppy or Bagel** image dataset (Kaggle)

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy, pandas
- Matplotlib, seaborn
- scikit-learn

## Key Results

From notebook outputs:
- Early epochs showed unstable training due to small dataset splits.
- Validation accuracy reached up to **1.0000** in some checkpoints.
- One captured test run reported **40.00% test accuracy**, highlighting variance and overfitting risk.

This project helped me see why robust data splitting and enough samples are critical for reliable generalization.

## Visual Results

See `results/`:
- `sample_training_images.png`
- `accuracy_loss_curves.png`
- `sample_predictions_grid.png`
- `confusion_matrix_resnet50.png`
- `visualization_inventory.md`

## What I Learned

- CNNs can memorize quickly on small datasets, so validation/test discipline matters.
- Transfer learning is often more stable than training from scratch for limited data.
- Confusion analysis is essential when class boundaries are visually subtle.

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook CNN_Puppy_vs_Bagel.ipynb
```
