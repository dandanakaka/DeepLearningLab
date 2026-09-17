# Experiment 1 — Single Layer Perceptron for Binary Classification

**Course:** CS3807 – Deep Learning Laboratory, Shiv Nadar University Chennai
**Degree & Branch:** B.Tech Artificial Intelligence & Data Science, Semester V

## Objective

Implement a single-layer perceptron from scratch and use it to perform binary classification, comparing the from-scratch implementation against scikit-learn's `Perceptron` and evaluating performance using standard classification metrics (accuracy, precision, recall, F1-score, confusion matrix).

## Dataset

**Banknote Authentication Dataset** (UCI Machine Learning Repository)

- 1,372 samples, 4 numeric features extracted from wavelet-transformed banknote images (variance, skewness, curtosis, entropy) plus a binary class label (genuine / forged).
- Loaded directly at runtime via URL inside the notebook — no manual download required.

## Repository Structure

```
01-single-layer-perceptron/
├── README.md                          # This file
├── single_layer_perceptron.ipynb      # Source code / experiment notebook
├── Lab_Report_Experiment1.pdf         # Full lab report
└── requirements.txt                   # Python dependencies
```

## Dependencies

See [`requirements.txt`](./requirements.txt). Key libraries:

- `numpy`, `pandas` — data handling
- `matplotlib`, `seaborn` — visualization (feature histograms, correlation heatmap, decision boundary, confusion matrix)
- `scikit-learn` — train/test split, feature scaling, evaluation metrics, and the reference `Perceptron` implementation

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
   jupyter notebook single_layer_perceptron.ipynb
   ```
   The notebook downloads the dataset automatically, so no additional setup is required.

## Contents Covered

- Dataset loading, exploration, and visualization (histograms, correlation heatmap, scatter plots, boxplots)
- Feature normalization and train/test split
- Perceptron implementation from scratch (weight/bias updates, training loop)
- Training error, weight, and bias evolution across epochs
- Evaluation via confusion matrix and standard classification metrics
- 2D decision boundary visualization
- Comparison against scikit-learn's `Perceptron`

## Author

Sidharth — B.Tech Artificial Intelligence & Data Science, Shiv Nadar University Chennai
