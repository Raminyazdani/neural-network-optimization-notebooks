# ML Optimization Techniques: PCA & Polynomial Regression

**Practical implementations of PCA-based dimensionality reduction, image denoising, and polynomial regression with regularization.**

**Stack:** Python, PyTorch, scikit-learn, Jupyter Notebook

## Overview

This project demonstrates two fundamental machine learning optimization techniques through hands-on Jupyter notebook implementations:
1. **Principal Component Analysis (PCA)** for dimensionality reduction and image denoising
2. **Polynomial Regression** with regularization for modeling non-linear relationships

The implementations provide both mathematical foundations and practical applications, making them useful for learning and reference.

## Problem & Approach

**Problem:** Machine learning practitioners often face challenges with high-dimensional data and overfitting in regression tasks. This project addresses: (1) reducing dimensionality while preserving essential information for tasks like image denoising, and (2) modeling non-linear relationships without overfitting.

**Approach:** 
- Implemented eigendecomposition and PCA from scratch to understand mathematical foundations
- Applied PCA for image reconstruction and denoising on MNIST handwritten digits
- Explored polynomial feature expansion for non-linear regression
- Compared linear regression, polynomial regression, and regularized models (Ridge, Lasso)
- Visualized reconstruction errors, variance explained, and model performance metrics

## Tech Stack

- Python 3.x
- PyTorch (deep learning framework)
- scikit-learn (machine learning library)
- Jupyter Notebook (interactive development)
- NumPy (numerical computing)
- Matplotlib (visualization)

## Repository Structure

```
ml-optimization-notebooks/
├── pca_image_denoising.ipynb      # PCA implementation and MNIST denoising
├── polynomial_regression.ipynb    # Polynomial regression with regularization
├── requirements.txt                # Python dependencies
├── data/                          # Data directory (for polynomial regression)
│   └── .gitkeep
└── README.md                      # This file
```

## Setup / Installation

1. Ensure Python 3.x is installed
2. Install required dependencies:

```bash
pip install -r requirements.txt
```

Or install individually:
```bash
pip install torch numpy matplotlib jupyter scikit-learn
```

## How to Run

1. Clone the repository and navigate to the project directory:
```bash
git clone https://github.com/Raminyazdani/neural-network-optimization-notebooks.git
cd neural-network-optimization-notebooks
```

2. Start Jupyter Notebook:
```bash
jupyter notebook
```

3. Open either notebook:
   - `pca_image_denoising.ipynb` - PCA implementation and image denoising on MNIST
   - `polynomial_regression.ipynb` - Polynomial regression analysis

4. Run cells sequentially from top to bottom

## Data / Inputs

**PCA & Image Denoising Notebook:**
- MNIST dataset (automatically downloaded via PyTorch/torchvision on first run)
- No manual data setup required

**Polynomial Regression Notebook:**
- Requires two numpy array files: `X.npy` and `y.npy`
- Place these files in the `data/` directory
- The notebook expects:
  - `data/X.npy` - Input features (1D or 2D array)
  - `data/y.npy` - Target values (1D array)
- If you don't have these files, you can generate synthetic data by running the data generation cells in the notebook

## Outputs

**PCA & Image Denoising:**
- PCA reconstructed images at various component counts
- Denoised images using PCA
- Reconstruction error plots
- Variance explained visualizations
- Eigenvalue distributions

**Polynomial Regression:**
- Trained regression models (linear, polynomial, regularized)
- RMSE comparisons across different model architectures
- Polynomial fit visualizations
- Overfitting analysis

## Reproducibility Notes

- Random seeds are set in notebooks for reproducible results
- All paths are relative to the project root directory
- Notebooks are self-contained with all function implementations
- MNIST data is automatically downloaded via PyTorch

## Troubleshooting

- **Import errors:** Ensure all dependencies are installed with `pip install -r requirements.txt`
- **Memory issues:** Reduce batch sizes or number of principal components in notebooks
- **PyTorch issues:** Verify installation with `python -c "import torch; print(torch.__version__)"`
- **Jupyter issues:** Ensure Jupyter is installed: `pip install jupyter`
- **Data file errors (polynomial regression):** Ensure `X.npy` and `y.npy` are in the `data/` directory
- **Path errors:** Run Jupyter from the project root directory

## Notes

- PCA implementation includes eigendecomposition from scratch for educational purposes
- Polynomial regression notebook demonstrates the bias-variance tradeoff
- All visualizations use Matplotlib for consistency
- Code follows PyTorch and scikit-learn best practices

