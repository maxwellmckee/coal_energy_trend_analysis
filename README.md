# Coal Energy Trend Analysis

## Overview
This repository presents an analysis of electrical energy produced by coal in the United States from 1950 to 2018. The project aims to model the mean function of the dataset using various regression techniques, including cubic splines, B-splines, smoothing splines, and kernel regression with a Gaussian kernel. The best model is selected based on the mean squared error (MSE) obtained through leave-one-out cross-validation (LOOCV). The results are visualized by plotting the data along with the fitted curve of the best model.

## Dependencies
* `numpy`: For handling numerical operations and arrays.
* `scipy`: Utilized for scientific computations, including optimization and spline fitting.
* `matplotlib`: For plotting and visualizing the data and fitted models.
* `skfda`: Used for functional data analysis, particularly for fitting B-splines and smoothing splines.

## Models and Validation
The project explores the following models to fit the energy production data:

* Cubic Splines: Varying the number of knots.
* B-splines: Varying the number of knots.
* Smoothing Splines: Selecting the optimal lambda (smoothing parameter).
* Kernel Regression: Employing a Gaussian kernel and selecting the optimal lambda.
* Leave-one-out cross-validation (LOOCV) is used across all models to compute the MSE, helping in selecting the best-performing model.

Results
The analysis concludes with the selection of the best model based on the lowest MSE. 
