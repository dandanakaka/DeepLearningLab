# Experiment 4 — Comparative Study of Deep CNN Architectures Using Transfer Learning

**Course:** CS3807 – Deep Learning Laboratory, Shiv Nadar University Chennai
**Degree & Branch:** B.Tech Artificial Intelligence & Data Science, Semester V

## Objective

Study the evolution of deep CNN architectures and apply transfer learning using a pretrained ImageNet backbone (ResNet50) to classify CIFAR-10 images, comparing feature extraction against fine-tuning.

## Dataset

**CIFAR-10** (via Hugging Face `datasets`)

- 60,000 32×32 RGB images across 10 classes, loaded using `load_dataset("uoft-cs/cifar10")` from the Hugging Face Hub.
- Downloaded automatically at runtime — requires an internet connection on first run; subsequent runs use the local Hugging Face cache.

## Repository Structure

```
04-transfer-learning-cnn-comparison/
├── README.md                                    # This file
├── transfer_learning_cnn_comparison.ipynb       # Source code / experiment notebook
├── Lab_Report_Experiment4.pdf                   # Full lab report
└── requirements.txt                             # Python dependencies
```

## Dependencies

See [`requirements.txt`](./requirements.txt). Key libraries:

- `numpy`, `pandas` — data handling
- `matplotlib` — visualization
- `torch`, `torchvision` — model definition (pretrained `ResNet50`), training loop, image transforms
- `datasets` (Hugging Face) — dataset loading

A CUDA-capable GPU is strongly recommended for reasonable training times, though the notebook will also run on CPU.

## Execution Instructions

1. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Launch Jupyter and run all cells top to bottom:
   ```bash
   jupyter notebook transfer_learning_cnn_comparison.ipynb
   ```
   The CIFAR-10 dataset is downloaded automatically from the Hugging Face Hub on first run.

## Contents Covered

- Loading CIFAR-10 via Hugging Face `datasets` and wrapping it in a PyTorch `Dataset`/`DataLoader`
- Dataset exploration and sample image visualization
- Loading a pretrained `ResNet50` (ImageNet weights) and freezing the convolutional base
- Replacing the classification head for CIFAR-10's 10 classes
- Comparing feature extraction (frozen backbone) vs. fine-tuning (unfrozen backbone)
- Training/validation performance comparison across architectures

## Author

Sidharth — B.Tech Artificial Intelligence & Data Science, Shiv Nadar University Chennai
