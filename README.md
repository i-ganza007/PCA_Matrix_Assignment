Principal Component Analysis (PCA) on Fuel Economy Dataset

Overview

This project performs Principal Component Analysis (PCA) on a fuel economy dataset to reduce dimensionality while preserving essential data patterns. The process includes data standardization, covariance matrix computation, eigen decomposition, and data projection onto principal components.

Requirements

Ensure you have the following Python packages installed:

pip install numpy pandas matplotlib

Dataset

The dataset used is fuel_econ-2.csv, which contains various fuel economy-related features. The numerical features are extracted for PCA analysis.

Steps Involved

Load Dataset

Read the CSV file into a Pandas DataFrame.

Extract numeric features and convert them into a NumPy array.

Standardization

Compute the mean and standard deviation.

Standardize the data by subtracting the mean and dividing by the standard deviation.

Compute Covariance Matrix

Calculate the covariance matrix of standardized data.

Eigen Decomposition

Compute eigenvalues and eigenvectors.

Sort eigenvalues in descending order and arrange eigenvectors accordingly.

Dimensionality Reduction

Select the top num_components (default is 2) eigenvectors.

Project data onto the selected principal components.

Visualization

Plot the original data (first two features) and the reduced data (first two principal components) using Matplotlib.

Output

The shape of the reduced data is printed.

The first 5 rows of transformed data are displayed.

Two scatter plots show a comparison between the original data and the PCA-transformed data.

Running the Script

Run the script using:

python pca_analysis.py

Ensure that fuel_econ-2.csv is in the correct directory.

Example Output

Reduced Data Shape: (num_samples, 2)
First 5 rows of the reduced data:
[[value1, value2]
 [value3, value4]
 ...]

Notes

PCA helps in reducing the dataset’s dimensions while retaining most of its variance.

The number of principal components can be adjusted as needed.

Ensure the dataset contains numerical values to avoid processing errors.

License

This project is open-source and available for educational purposes.
