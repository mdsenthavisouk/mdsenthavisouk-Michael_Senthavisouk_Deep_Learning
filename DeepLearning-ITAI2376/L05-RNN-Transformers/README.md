# L05 — RNNs vs Transformers vs Vision Transformers

## Project Overview

In this comprehensive lab, I compared multiple sequence and vision architectures side-by-side:
- Vanilla RNN / LSTM / GRU for text
- DistilBERT for transformer-based text classification
- ViT for image classification

## Problem Statement

I wanted to measure the tradeoffs between model families in terms of accuracy, training dynamics, and computational cost across NLP and vision tasks.

## My Approach

### Part A/B (Text Classification)
- Prepared AG News-style text pipeline (tokenization, vocabulary, sequence padding)
- Trained and evaluated RNN, LSTM, and GRU classifiers
- Fine-tuned a **DistilBERT** model for comparison

### Part C (Vision)
- Trained/evaluated a **Vision Transformer (ViT)** workflow on CIFAR-10 scale data
- Compared performance trends with prior CNN experience

## Datasets

- **AG News** (via Hugging Face datasets tooling)
- **CIFAR-10**

## Technologies Used

- Python
- PyTorch
- Hugging Face `datasets` and `transformers`
- torchvision
- NumPy, pandas
- Matplotlib

## Key Results

Captured outputs show:
- Vanilla RNN test performance around **0.7450**
- LSTM/GRU improvements around **0.7775–0.8130**
- DistilBERT test accuracy around **0.90+** (peaks near **0.9070**)

This confirms the practical advantage of transformer-based models on text understanding tasks.

## Visual Results

See `results/` for extracted figures (12 key images) and inventory details.

## What I Learned

- Sequence architecture matters: GRU/LSTM generally outperformed vanilla RNN.
- Transformers provided the strongest NLP performance in this lab.
- Benchmarking multiple models on aligned tasks gave me clearer architectural intuition.

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook RNN_Transformers_Comparison.ipynb
```

GPU is strongly recommended for the transformer sections.
