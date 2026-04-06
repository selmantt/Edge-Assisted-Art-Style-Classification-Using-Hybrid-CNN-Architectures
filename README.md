# Edge-Assisted Art Style Classification Using Hybrid CNN Architectures

A computer vision project that classifies fine-art paintings by style (e.g., Impressionism, Baroque, Cubism) using hybrid Convolutional Neural Network architectures enhanced with edge-detection preprocessing, designed for deployment on edge devices.

## Overview

Automated art style classification is a challenging task due to high intra-class variability and the subtle visual cues that distinguish artistic movements. This project combines classical edge-detection filters (Sobel, Canny) with modern CNN backbones (ResNet, EfficientNet) in a hybrid dual-stream architecture that processes both raw RGB pixels and edge-feature maps simultaneously.

## Key Features

- **Dual-stream input:** RGB image stream + edge-feature stream merged at the classification head
- **Hybrid CNN backbones:** Pretrained ResNet / EfficientNet with fine-tuned final layers
- **Edge preprocessing:** Sobel and Canny filters applied at inference time — no extra training data needed
- **Edge deployment focus:** Model size and inference time optimized for resource-constrained hardware
- **Evaluated on WikiArt dataset:** Multi-class classification across major Western art movements

## Methodology

1. Preprocessing: resize, normalize, extract edge maps
2. Feature extraction: dual CNN streams (RGB + edges) run in parallel
3. Fusion: concatenate feature vectors before the classification head
4. Training: cross-entropy loss, Adam optimizer, learning rate scheduling
5. Evaluation: Top-1 accuracy, confusion matrix, per-class F1

## Project Structure

```
├── Project Report.pdf  # Full technical report with architecture diagrams and results
├── README.md
└── LICENSE
```

## Technologies

Python · PyTorch · torchvision · OpenCV · NumPy · Matplotlib

## License

MIT


