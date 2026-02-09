Project Overview – PCA on African Malaria Data

Objective:
For this sophisticated linear algebra implementation task (Formative 1), we will implement Principal Component Analysis (PCA) from scratch using only the NumPy library. The goal is to reduce the dimensionality of real-world African malaria data while preserving the maximum amount of information using eigenvalues, eigenvectors, and covariance matrices.

Dataset: malaria_data_db_format.csv

What the Data Represents:

African countries’ malaria outbreak statistics

Multiple features (over ten) including demographic, environmental, and epidemiological indicators

Contains missing values

Includes some non-numerical columns that will need preprocessing

Real-world, non-simulated data

How PCA Works (Linear Algebra Approach)

This PCA implementation follows the traditional linear algebra workflow, without using machine learning libraries:

Data Standardization
Normalize features so that each has mean 0 and standard deviation 1, using:

This step ensures that features with different scales contribute equally to PCA.

Covariance Matrix Calculation
Compute the covariance matrix with NumPy to understand how features relate to each other and identify correlated variables.

Eigenvalues and Eigenvectors

Eigenvalues measure how much variance each principal component explains

Eigenvectors indicate the directions along which the variance is maximal

Assembling Principal Components

Sort eigenvalues in descending order and pair them with their eigenvectors

PC1 explains the most variance

Subsequent PCs explain progressively less

Projection onto Principal Components
Project the standardized data onto the chosen principal components to reduce dimensionality.

Visualization

Plot the first two original standardized features for comparison

Plot the data in the PC1–PC2 space after PCA

Helps evaluate variance preserved and dimensionality reduction achieved

Technologies Used

Python – core language for computation

NumPy – matrix operations, covariance, eigenvalues/eigenvectors

Pandas – data loading, cleaning, and preprocessing

Matplotlib – visualization of original and PCA-transformed data
https://colab.research.google.com/drive/1z4l1hw5QAp0gn-ugk6CWjd165vGJ250R?usp=sharing
