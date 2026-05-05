# L08 — Diffusion Models for Image Generation

## Project Overview

In this lab, I implemented and trained a diffusion-based generative model to create images from noise. The core idea was to learn a denoising process that gradually reconstructs meaningful digits/images.

## Problem Statement

I explored how diffusion models can generate realistic samples by reversing a noise process, and how training stability evolves across optimization steps.

## My Approach

1. Set up diffusion training pipeline in PyTorch
2. Trained on lightweight image data (MNIST-centered workflow)
3. Monitored training/validation loss over multiple epochs
4. Sample outputs at progressive denoising stages

## Datasets

- **MNIST** (primary)
- Optional extensions in notebook: **Fashion-MNIST**, **CIFAR-10**

## Technologies Used

- Python
- PyTorch / torchvision
- NumPy
- Matplotlib
- PIL
- Supporting libraries: einops, clip (optional sections)

## Key Results

From notebook logs:
- Training loss decreased from roughly **0.0819** to around **0.0606** over sampled steps.
- Validation loss improved across epochs (e.g., **0.0679 → 0.0645**).
- Multiple image grids showed clearer structure as denoising progressed.

## Visual Results

See `results/` for extracted denoising and generation images (12 key PNGs) plus inventory documentation.

## What I Learned

- Diffusion models are computationally heavier but provide controllable generation behavior.
- Monitoring both training and validation loss helped me catch stability shifts.
- Visual checkpoints are essential for evaluating generative quality beyond numeric loss.

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook Diffusion_Models_Image_Generation.ipynb
```

Use GPU runtime for practical training speed.
