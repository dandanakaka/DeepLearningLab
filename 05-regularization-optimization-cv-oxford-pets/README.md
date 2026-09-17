# Experiment 5 — Regularization, Optimization, and Cross-Validation on Oxford-IIIT Pet Dataset Using Transfer Learning

**Course:** CS3807 – Deep Learning Laboratory, Shiv Nadar University Chennai
**Degree & Branch:** B.Tech Artificial Intelligence & Data Science, Semester V

## Objective

Investigate the effects of weight initialization, regularization (L2, dropout, batch normalization), optimizer choice, and hyperparameter tuning on a transfer-learning image classifier, and validate the best configuration using 5-fold cross-validation.

## Dataset

**Oxford-IIIT Pet Dataset**

- 37 categories of cat and dog breeds (~7,400 images total), loaded via `tensorflow_datasets` (`tfds`).
- Downloaded automatically at runtime by `tensorflow-datasets` — no manual download required, but the first run needs an internet connection to fetch and cache the dataset.

## Repository Structure

```
05-regularization-optimization-cv-oxford-pets/
├── README.md                            # This file
├── regularization_optimization_cv.ipynb # Source code / experiment notebook
├── Lab_Report_Experiment5.pdf           # Full lab report
└── requirements.txt                     # Python dependencies
```

## Dependencies

See [`requirements.txt`](./requirements.txt). Key libraries:

- `numpy` — array operations
- `matplotlib` — extensive plotting (15 result plots across all studies)
- `tensorflow` (Keras) — `MobileNetV2` transfer-learning base and model training
- `tensorflow-datasets` — Oxford-IIIT Pet dataset loading
- `scikit-learn` — cross-validation utilities

A GPU is strongly recommended, since the notebook trains multiple models across six separate studies plus a 5-fold cross-validation pass.

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
   jupyter notebook regularization_optimization_cv.ipynb
   ```
   The Oxford-IIIT Pet dataset is downloaded automatically via `tensorflow-datasets` on first run.

## Contents Covered

1. **Data pipeline** — loading and preprocessing the Oxford-IIIT Pet dataset with `tf.data`
2. **Study 1 — Weight Initialization**: Zeros, Random Normal, Xavier/Glorot, He Normal
3. **Study 2 — Regularization**: No regularization, L2, Dropout, Batch Normalization
4. **Study 3 — Batch Normalization**: with vs. without
5. **Study 4 — Optimizers**: SGD, Momentum, RMSProp, Adam
6. **Study 5 — Hyperparameter Tuning**: learning rate, batch size, dropout rate sweeps
7. **Study 6 — Feature Extraction vs. Fine-Tuning** using a `MobileNetV2` backbone pretrained on ImageNet
8. **5-Fold Cross-Validation** to select the best-performing configuration
9. **Final model evaluation** on the held-out test set with accuracy/loss metrics and confusion matrix

## Author

Sidharth — B.Tech Artificial Intelligence & Data Science, Shiv Nadar University Chennai
