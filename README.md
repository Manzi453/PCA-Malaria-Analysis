Project overview

For this sophisticated linear algebra implementation task, Formative 1, we will create Principal Component Analysis from scratch using only the NumPy library. The goal is to minimize the dimensionality of real-world African data while preserving the greatest amount of information by using eigenvalues, eigenvectors, and covariance matrices.
Dataset: ebola_data_db_format.csv What the data is
Background: African countries' Ebola outbreak statistics.
QualitiesOver ten in quantity
There are missing values in this

Inherently non-numerical

Actual data, not simulated or fake
How the method functions
Without the use of sophisticated machine learning libraries, this PCA adheres to the traditional linear algebra workflow.
1) Data standardisation

Normalize the features by computing z = (x – μ) / σ such that:

- Mean becomes 0

- Standard Deviation becomes 1

This normalisation is vital for the implementation of PCA based on covariance.

2. Covariance Matrix

Next, we calculate the covariance matrix using NumPy and show how the different features relate.

3) Eig

To better understand where the data's variance is and where the most important directions lie using eigenvalues and eigenvectors:

- Eigenvalues measure the amount of variance explained

- Eigenvectors show us the major directions

4) Assembling the components

First, arrange the eigenvalues in descending order and pair them with their corresponding eigenvectors:

- PC1 accounts for the most variance

- The following PCs explain progressively less variance

5) Project onto principal components

Project the standardized data onto the selected principal components.

6. Visualization
- In the original space, visualize using the first two standardized features
- After applying the PCA, plot in the PC1–PC2 space
This method enables you to determine the measure of variance maintained and dimensionality reduced. Technologies Involved - Python - NumPy (matrix operations, covariance, eigendecom - Pandas (data loading and preprocessing) - Matplotlib for Visualization