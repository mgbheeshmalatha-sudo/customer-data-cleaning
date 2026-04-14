# customer-data-cleaning
Customer Data Cleaning and Feature Engineering
This repository contains a Python-based data preprocessing pipeline designed to handle raw, "messy" customer datasets. The project demonstrates essential data science workflows, including missing value imputation, duplicate removal, categorical encoding, and feature scaling.

Project Overview
The goal of this project is to transform a raw dataset with inconsistent entries into a clean, machine-learning-ready format.

Key Tasks Performed:
Data Cleaning:

Imputed missing age values using the Median.

Imputed missing city values using the Mode.

Identified and removed duplicate records to ensure data integrity.

Categorical Encoding:

Converted the city column into numerical format using One-Hot Encoding.

Converted the gender column using Label Encoding.

Feature Scaling:

Applied Min-Max Scaling to compress numerical features into a range of [0, 1].

Applied Standardization to center features around a mean of 0 with unit variance.

Installation & Requirements
To run the notebook locally, you will need Python 3.x and the following libraries:

Bash
pip install pandas numpy scikit-learn
Scaling Methodology: Comparison
One of the critical steps in this pipeline is comparing two scaling methods:

Min-Max Scaling: Preferred when the data distribution is not Gaussian and you need a bounded range (0 to 1). It is often used in algorithms like Neural Networks or K-Nearest Neighbors.

Standardization (Z-score): Preferred when the data follows a Normal/Gaussian distribution or when using algorithms that assume centered data (like PCA, SVM, or Linear Regression). It is generally more robust to outliers than Min-Max scaling.


Run the cells to see the transformation from raw data to the final processed dataframe.
