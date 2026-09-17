# Experiment 3 — Convolutional Neural Networks (CNNs) for Image Classification

**Course:** CS3807 – Deep Learning Laboratory, Shiv Nadar University Chennai
**Degree & Branch:** B.Tech Artificial Intelligence & Data Science, Semester V

## Objective

Understand the working principles of Convolutional Neural Networks by implementing convolution operations (filters, strides, padding) manually, then build and train a CNN classifier on the CIFAR-10 dataset.

## Dataset

**CIFAR-10**

- 60,000 32×32 RGB images across 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck) — 50,000 training / 10,000 test images.
- Downloaded automatically at runtime via `tf.keras.datasets.cifar10.load_data()` — no manual download required.

## Repository Structure

```
03-cnn-image-classification/
├── README.md                        # This file
├── cnn_image_classification.ipynb   # Source code / experiment notebook
├── Lab_Report_Experiment3.pdf       # Full lab report
└── requirements.txt                 # Python dependencies
```

## Dependencies

See [`requirements.txt`](./requirements.txt). Key libraries:

- `numpy` — array/tensor operations for manual convolution demos
- `matplotlib`, `seaborn` — visualization (sample images, class distribution, feature maps, confusion matrix)
- `tensorflow` (Keras) — CNN model definition and training
- `scikit-learn` — classification report and confusion matrix

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
   jupyter notebook cnn_image_classification.ipynb
   ```
   CIFAR-10 is downloaded automatically by TensorFlow on first run.

## Contents Covered

- Loading and visualizing CIFAR-10 (sample images, class distribution)
- Manual implementation of convolution operations with varying kernel size, stride, and padding
- Visualizing learned feature maps from a `Conv2D` layer
- Building and training a CNN classifier in Keras
- Training/validation accuracy and loss curves
- Evaluation via classification report and confusion matrix

## Author

Sidharth — B.Tech Artificial Intelligence & Data Science, Shiv Nadar University Chennai
