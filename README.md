# Principal Component Analysis (PCA) on Fuel Economy Dataset

## Overview
This project performs Principal Component Analysis (PCA) on a fuel economy dataset to reduce dimensionality while preserving essential data patterns. The process includes:
- Data standardization
- Covariance matrix computation
- Eigen decomposition
- Data projection onto principal components

## Dataset
The dataset used is `fuel_econ-2.csv`, which contains various fuel economy-related features. The numerical features are extracted for PCA analysis.

## Requirements
Install the necessary Python libraries using:
```bash
pip install numpy pandas matplotlib
```

## Steps Involved

### 1. Load Dataset
- Read the CSV file into a Pandas DataFrame.
- Extract numeric features and convert them into a NumPy array.

### 2. Standardization
- Compute the mean and standard deviation.
- Standardize the data by subtracting the mean and dividing by the standard deviation.

### 3. Compute Covariance Matrix
- Calculate the covariance matrix of standardized data.

### 4. Eigen Decomposition
- Compute eigenvalues and eigenvectors.
- Sort eigenvalues in descending order and arrange eigenvectors accordingly.

### 5. Dimensionality Reduction
- Select the top `num_components` (default is 2) eigenvectors.
- Project data onto the selected principal components.

### 6. Visualization
- Plot the original data (first two features) and the reduced data (first two principal components) using Matplotlib.

## Running the Script
Run the script using:
```bash
python pca_analysis.py
```
Ensure that `fuel_econ-2.csv` is in the correct directory.

## Output
- The shape of the reduced data is printed.
- The first 5 rows of transformed data are displayed.
- Two scatter plots show a comparison between the original data and the PCA-transformed data.

### Example Output
```bash
Reduced Data Shape: (num_samples, 2)
First 5 rows of the reduced data:
[[value1, value2]
 [value3, value4]
 ...]
```

## Notes
- PCA helps in reducing the dataset’s dimensions while retaining most of its variance.
- The number of principal components can be adjusted as needed.
- Ensure the dataset contains numerical values to avoid processing errors.

## License
This project is open-source and available for educational purposes.

