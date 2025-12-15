# 🌫️ ELKAformer Image Dehazing System

A Transformer-based single image dehazing system implemented using PyTorch and the ELKAformer architecture.  
This project focuses on restoring clear images from haze-degraded inputs using an end-to-end deep learning pipeline.

---

## Overview

This project implements a high-quality image dehazing solution using a transformer-based restoration model.  
It learns a mapping between hazy images and their corresponding ground-truth clear images and produces visually sharp and structurally accurate results.

Key features:
- Single-image atmospheric haze removal
- Transformer-based ELKAformer architecture
- Complete training, testing, evaluation, and visualization pipeline
- Quantitative evaluation using PSNR and SSIM

---

## Model Architecture

- Architecture: ELKAformer (Transformer-based Image Restoration Network)
- Input Channels: 3 (RGB)
- Output Channels: 3 (RGB)
- Image Resolution: 256 × 256
- Feature Dimension (dim): 36
- Encoder–Decoder Blocks: [3, 4, 4, 6]
- Refinement Blocks: 3
- FFN Expansion Factor: 2.66

---

## Training Configuration

- Loss Function: Charbonnier Loss
- Optimizer: AdamW
- Learning Rate: 1e-4
- Weight Decay: 1e-4
- Learning Rate Scheduler: Cosine Annealing
- Gradient Clipping: Enabled (max norm = 1.0)
- Training Epochs: 300
- Batch Size: 1





