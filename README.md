# Machine Learning Practice in MATLAB

## Overview

This academic repository presents a complete machine learning study using MATLAB, applying and comparing different classification and regression algorithms. The work spans from traditional classifiers to neural networks and chaotic time series modeling. The goal is to assess model performance through rigorous cross-validation and statistical methods, across multiple problem types.

## Objectives

- Train and compare classifiers:
  - Linear Discriminant Analysis (LDA)
  - Quadratic Discriminant Analysis (QDA)
  - Decision Trees
  - Support Vector Machines (SVM) with multiple kernels and C values
  - Artificial Neural Networks (ANN) for binary classification
- Evaluate regression models:
  - Applied to time series generated from the Hénon map
- Use proper validation strategies:
  - LOOCV (Iris)
  - Repeated K-Fold CV (QSAR)
- Evaluate with:
  - Accuracy, Precision, Recall, Specificity, F1-Score (classification)
  - Mean Squared Error (MSE) and visual comparison (regression)
- Conduct statistical tests:
  - Kruskal-Wallis test with Bonferroni correction

## Datasets

- **Iris Dataset**: 150 samples of flower measurements with 3 classes.
- **QSAR Biodegradation Dataset**: 1055 molecules labeled as biodegradable/non-biodegradable.
- **Hénon Time Series**: Synthetic data generated from a chaotic system for regression tasks.

All datasets are located under the `data/` directory.

## Project Structure

```text
data/
├── IrisDataset/                 # Iris data
├── QSARDataset/                 # QSAR descriptors
├── henon.m                      # Hénon map generator (provided)

src/
├── P3Iris.mlx                   # LOOCV classifiers on Iris
├── P3QSAR.mlx                   # CV classifiers on QSAR
├── P4IrisCV.mlx                 # SVM classifiers on Iris
├── P4QSAR.mlx                   # SVM classifiers on QSAR
├── P3_2.mlx                     # ANN applied to QSAR
├── P4_2.mlx                     # Regression with Hénon data
├── performanceIndexes.m        # Provided: computes confusion-matrix metrics
├── slidingwindow.m             # Provided: cross-validation fold manager

LICENSE
README.md
memory.pdf                       # Final report with analysis and results
