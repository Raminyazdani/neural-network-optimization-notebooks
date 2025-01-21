# Project Identity

## Display Title
ML Optimization Techniques: PCA & Polynomial Regression

## Repo Slug
ml-optimization-notebooks

## Tagline
Practical implementations of PCA-based dimensionality reduction, image denoising, and polynomial regression with regularization.

## GitHub Description
A collection of Jupyter notebooks demonstrating principal component analysis (PCA) for image denoising on MNIST data and polynomial regression with regularization techniques, implemented in PyTorch and scikit-learn.

## Primary Stack
- Python
- PyTorch
- scikit-learn
- Jupyter Notebook
- NumPy
- Matplotlib

## Topics/Keywords
- machine-learning
- pca
- dimensionality-reduction
- image-denoising
- polynomial-regression
- regularization
- pytorch
- scikit-learn
- jupyter-notebook
- mnist
- data-science

## Problem & Solution

### Problem
Machine learning practitioners often face challenges with high-dimensional data and overfitting in regression tasks. This project addresses two common scenarios: (1) reducing dimensionality while preserving essential information for tasks like image denoising, and (2) modeling non-linear relationships without overfitting.

### Approach
This project provides hands-on implementations and analysis of:
- Eigendecomposition and PCA from scratch to understand mathematical foundations
- PCA application for image reconstruction and denoising on MNIST handwritten digits
- Polynomial feature expansion for non-linear regression
- Model comparison: linear regression vs. polynomial regression vs. regularized models (Ridge, Lasso)
- Visualization of reconstruction errors, variance explained, and model performance metrics

## Inputs & Outputs

### Inputs
- MNIST handwritten digit images (loaded via PyTorch/torchvision)
- Optional: Custom regression dataset (X.npy, y.npy files for polynomial regression experiments)

### Outputs
- PCA reconstructed images at various component counts
- Denoised images using PCA techniques
- Reconstruction error plots and variance explained visualizations
- Trained regression models (linear, polynomial, regularized)
- RMSE comparisons across different model architectures
- Polynomial fit visualizations

