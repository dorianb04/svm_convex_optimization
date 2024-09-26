# Optimization of Support Vector Machines (SVM)

## Project Overview
This project explores the optimization of Support Vector Machines (SVMs) for binary classification tasks. Focusing on gradient-based methods, we compare the performance of Subgradient Method, Proximal Gradient Descent, and the Fast Iterative Shrinkage-Thresholding Algorithm (FISTA). Our aim is to enhance computational efficiency and accuracy in SVM training, particularly for large datasets.

## Motivation
The challenge of efficiently training SVMs, especially when confronted with large and complex datasets, is a key issue in machine learning. This project seeks to address this challenge by evaluating and comparing various optimization algorithms, each with their unique approach to handling the non-smooth hinge loss function intrinsic to SVMs.

## Datasets
The primary dataset used in this study is the [Pima Indians Diabetes Database](https://www.kaggle.com/uciml/pima-indians-diabetes-database), consisting of diagnostic measurements from 768 female patients of Pima Indian heritage.

## Methods
- **Subgradient Method**: Tackles the non-differentiability of the hinge loss function in SVMs.
- **Proximal Gradient Descent**: Combines gradient descent for the smooth part of the SVM loss with a proximal step for the hinge loss.
- **FISTA**: An advanced variant of Proximal Gradient Descent, introducing acceleration steps to hasten convergence.

## Results
The methods were evaluated based on training loss, accuracy, execution time, and test accuracy. Detailed results and visualizations can be found in the [`results`](/results) directory.

Optimization Algorithm            |  Training
:-------------------------:|:-------------------------:
**Subgradient Descent** |  ![](/results/Subgradient%20Method.png) 
**Proximal Gradient Descent**| ![](results/Proximal%20Gradient%20Descent.png)  
**FISTA** | ![](/results/FISTA.png)

## Dependencies
- NumPy
- Pandas
- Matplotlib
- Scikit-learn (only for using PCA to create visualization of the Dataset)

## Author
- **Boucher Dorian** - *Initial Work* - [dorian.bch44@gmail.com](mailto:dorian.bch44@gmail.com)
