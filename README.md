# Deep Learning Laboratory

Official repository for the **CS3807 – Deep Learning Laboratory** experiments, Semester V, B.Tech Artificial Intelligence & Data Science, Shiv Nadar University Chennai.

Each experiment lives in its own folder with a self-contained notebook, lab report, dataset information, dependency list, and execution instructions.

## Experiments

| # | Folder | Title | Dataset | Framework |
|---|--------|-------|---------|-----------|
| 1 | [`01-single-layer-perceptron`](./01-single-layer-perceptron) | Single Layer Perceptron for Binary Classification | Banknote Authentication (UCI) | NumPy / scikit-learn |
| 2 | [`02-multi-layer-perceptron`](./02-multi-layer-perceptron) | Multi-Layer Perceptron for Multi-Class Image Classification | Fashion-MNIST | TensorFlow / Keras |
| 3 | [`03-cnn-image-classification`](./03-cnn-image-classification) | Convolutional Neural Networks for Image Classification | CIFAR-10 | TensorFlow / Keras |
| 4 | [`04-transfer-learning-cnn-comparison`](./04-transfer-learning-cnn-comparison) | Comparative Study of Deep CNN Architectures Using Transfer Learning | CIFAR-10 (Hugging Face) | PyTorch (ResNet50) |
| 5 | [`05-regularization-optimization-cv-oxford-pets`](./05-regularization-optimization-cv-oxford-pets) | Regularization, Optimization, and Cross-Validation on Oxford-IIIT Pet Dataset | Oxford-IIIT Pet | TensorFlow / Keras (MobileNetV2) |

## Repository Structure

```
DeepLearningLab/
├── 01-single-layer-perceptron/
│   ├── README.md
│   ├── single_layer_perceptron.ipynb
│   ├── Lab_Report_Experiment1.pdf
│   └── requirements.txt
├── 02-multi-layer-perceptron/
│   ├── README.md
│   ├── multi_layer_perceptron.ipynb
│   ├── Lab_Report_Experiment2.pdf
│   └── requirements.txt
├── 03-cnn-image-classification/
│   ├── README.md
│   ├── cnn_image_classification.ipynb
│   ├── Lab_Report_Experiment3.pdf
│   └── requirements.txt
├── 04-transfer-learning-cnn-comparison/
│   ├── README.md
│   ├── transfer_learning_cnn_comparison.ipynb
│   ├── Lab_Report_Experiment4.pdf
│   └── requirements.txt
├── 05-regularization-optimization-cv-oxford-pets/
│   ├── README.md
│   ├── regularization_optimization_cv.ipynb
│   ├── Lab_Report_Experiment5.pdf
│   └── requirements.txt
└── README.md
```

## Getting Started

Each experiment folder is independent and has its own `requirements.txt` and execution instructions in its README. General workflow:

```bash
git clone https://github.com/dandanakaka/DeepLearningLab.git
cd DeepLearningLab/<experiment-folder>
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook <notebook-name>.ipynb
```

## Author

Sidharth — B.Tech Artificial Intelligence & Data Science, Shiv Nadar University Chennai
