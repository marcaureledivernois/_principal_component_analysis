## Principal Component Anaylisis

## Overview

Unsupervised. Dimensionality reduction. 
Feature extraction technique consisting of finding new features after transforming the data from
a high dimensional space to a lower dimensional space.
Discover non-linear non-local relationships in data that are not in the original
feature space.

## How does it work ?

Orthogonal linear transformation that transforms data to a new coordinate system such that
the greatest ("2nd) variance by some projection of the data lies on the first (2nd) component, etc.
It is a variance maximizing exercise, it projects the data onto a direction which maximizes variance.

## Eigenvectors, Eigenvalues

Eigen is a german word that roughly translates to "characteristic". 
An eigenvector is a vector that does not change its direction and length under the associated linear transformation.

Av = &lambda;v

with A some matrix, v the eigenvector and &lambda; the associated eigenvalue

An eigenpair is the eigenvalue and its associated eigenvector.

## Steps

1. Standardize data
2. Eigendecomposition of the covariance matrix
3. Select the P (e.g. 2) highest eigenpairs
4. Construct the projection matrix w (= concatenated top P eigenvectors)
5. Transform the original data onto the new subspace (dot product : data*w)

## Use cases

* Feature selection (avoid overfitting, reduce computing time, reduce complexity)
* Data visualization (possible to plot data in 2D or 3D)

## Credits

* Siraj Raval
* Disclaimer : Code is used as an illustration of the README theory file. Code has been forked from [rasbt](https://github.com/rasbt). I mainly corrected/updated it to make it work on my computers.
