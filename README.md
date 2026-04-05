# Edge-Assisted Art Style Classification Using Hybrid CNN Architectures

A deep learning research project exploring the use of **edge-detected image features** combined with **hybrid Convolutional Neural Network (CNN)** architectures for classifying art styles.

## Overview

Art style classification is a challenging task due to the subjective and overlapping nature of artistic movements. This project proposes a hybrid approach that fuses:
- **RGB image features** for color and texture information
- **Edge-detected features** (e.g., Canny, Sobel) for structural and compositional cues

By providing edge maps as an auxiliary input channel, the model captures compositional patterns that are characteristic of different artistic movements, achieving improved classification over standard single-stream CNNs.

## Project Structure

```
├── Project Report.pdf    # Full project report with methodology, experiments, and results
├── LICENSE               # MIT License
└── README.md
```

## Report Highlights

The `Project Report.pdf` contains:
- Literature review on CNN-based art classification
- Methodology for edge extraction and hybrid architecture design
- Comparative experiments between single-stream and dual-stream CNN models
- Results analysis with accuracy metrics and confusion matrices

