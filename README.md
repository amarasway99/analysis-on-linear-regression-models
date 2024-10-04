# Analysis on Linear Regression Models

This repository contains the analysis of both regularized and non-regularized Newton methods for linear regression. The project includes error computation, performance evaluation, and experimentation with different regularization parameters and train-test splits.

## Project Overview

The project is structured into several key steps:

### 1. **Newton Method**
   - Matrix computation: \( (X'X)^{-1} X'y \)
   - Used rows 2 to 41 from the dataset for training data.
   - Computed weights \( w \), generated predicted y values, and evaluated model performance using Sum of Squared Residuals (SSR), Mean Squared Residuals (MSR), and Root Mean Squared Error (RMSE).
   - Errors computed for both training (rows 2 to 41) and test data (rows 43 to 51).

### 2. **Regularized Newton Method**
   - Matrix computation: \( (X'X + \lambda I)^{-1} X'y \)
   - Regularization applied with \( \lambda = 0.17 \).
   - Errors computed for both training (rows 2 to 41) and test data (rows 43 to 51).

### 3. **R-squared Evaluation**
   - Computed R-squared values for both Newton and Regularized Newton methods on both the training and test datasets.

### 4. **Additional Experimentation**
   The following variations were explored, and MSR (Mean Squared Residuals) and R-squared values were reported for both training and test datasets:
   - Use rows 2 to 41 for training and rows 42 to 51 for testing with \( \lambda = 0.83 \).
   - Use rows 2 to 26 for training and rows 27 to 51 for testing with \( \lambda = 0.17 \).
   - Use rows 2 to 26 for training and rows 27 to 51 for testing with \( \lambda = 0.83 \).
   - Use rows 2 to 11 for training and rows 12 to 51 for testing with \( \lambda = 0.17 \).
   - Use rows 2 to 11 for training and rows 12 to 51 for testing with \( \lambda = 0.83 \).

## Requirements

To run the code in this repository, ensure the following Python modules are installed:

```bash
pip install pandas
pip install openpyxl
pip install scikit-learn
