# Experiment 2 — Multi-Layer Perceptron (MLP) for Multi-Class Image Classification

**Course:** CS3807 – Deep Learning Laboratory, Shiv Nadar University Chennai
**Degree & Branch:** B.Tech Artificial Intelligence & Data Science, Semester V

## Objective

Implement a Multi-Layer Perceptron using TensorFlow/Keras to classify grayscale clothing images into 10 categories, and tune network hyperparameters via randomized search to identify the best-performing configuration.

## Dataset

**Fashion-MNIST**

- 70,000 grayscale 28×28 images across 10 clothing categories (T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot).
- Supplied as CSV files (`fashion-mnist_train.csv`, `fashion-mnist_test.csv`) inside a zip archive. Place the archive as `archive.zip` in the working directory (or update the path in the notebook's extraction cell) before running.
- Original source: [Fashion-MNIST on Kaggle](https://www.kaggle.com/datasets/zalando-research/fashionmnist) / [Zalando Research GitHub](https://github.com/zalandoresearch/fashion-mnist).

## Repository Structure

```
02-multi-layer-perceptron/
├── README.md                       # This file
├── multi_layer_perceptron.ipynb    # Source code / experiment notebook
├── Lab_Report_Experiment2.pdf      # Full lab report
└── requirements.txt                # Python dependencies
```

## Dependencies

See [`requirements.txt`](./requirements.txt). Key libraries:

- `numpy`, `pandas` — data handling
- `matplotlib`, `seaborn` — visualization
- `tensorflow` (Keras) — MLP model definition and training
- `scikit-learn`, `scikeras` — `RandomizedSearchCV` hyperparameter tuning of the Keras model

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
3. Download the Fashion-MNIST CSV dataset (see [Dataset](#dataset) above) and place the zip archive where the notebook expects it (update the `zip_file_path` variable near the top of the notebook if needed).
4. Launch Jupyter and run all cells top to bottom:
   ```bash
   jupyter notebook multi_layer_perceptron.ipynb
   ```

## Contents Covered

- Extracting and loading the Fashion-MNIST CSV dataset
- Data exploration and sample image visualization
- MLP architecture definition using Keras `Sequential`/functional API
- Randomized hyperparameter search (`RandomizedSearchCV` via `scikeras`) over layer sizes, activation functions, learning rate, etc.
- Model evaluation with classification report and confusion matrix
- Visualization of hyperparameter search results

## Author

Sidharth — B.Tech Artificial Intelligence & Data Science, Shiv Nadar University Chennai
