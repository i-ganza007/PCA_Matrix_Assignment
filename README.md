<!-- README.md -->

<!DOCTYPE html>
<html>
<head>
    <title>Principal Component Analysis (PCA) on Fuel Economy Dataset</title>
    <style>
        body { font-family: Arial, sans-serif; line-height: 1.6; margin: 40px; }
        h1, h2, h3 { color: #2c3e50; }
        code { background-color: #f4f4f4; padding: 2px 5px; border-radius: 4px; }
        pre { background-color: #f4f4f4; padding: 10px; border-radius: 4px; overflow-x: auto; }
        ul { margin: 10px 0; padding-left: 20px; }
    </style>
</head>
<body>
    <h1>Principal Component Analysis (PCA) on Fuel Economy Dataset</h1>
    
    <h2>Overview</h2>
    <p>This project performs Principal Component Analysis (PCA) on a fuel economy dataset to reduce dimensionality while preserving essential data patterns. The process includes data standardization, covariance matrix computation, eigen decomposition, and data projection onto principal components.</p>
    
    <h2>Requirements</h2>
    <p>Ensure you have the following Python packages installed:</p>
    <pre><code>pip install numpy pandas matplotlib</code></pre>
    
    <h2>Dataset</h2>
    <p>The dataset used is <code>fuel_econ-2.csv</code>, which contains various fuel economy-related features. The numerical features are extracted for PCA analysis.</p>
    
    <h2>Steps Involved</h2>
    <h3>1. Load Dataset</h3>
    <ul>
        <li>Read the CSV file into a Pandas DataFrame.</li>
        <li>Extract numeric features and convert them into a NumPy array.</li>
    </ul>
    
    <h3>2. Standardization</h3>
    <ul>
        <li>Compute the mean and standard deviation.</li>
        <li>Standardize the data by subtracting the mean and dividing by the standard deviation.</li>
    </ul>
    
    <h3>3. Compute Covariance Matrix</h3>
    <ul>
        <li>Calculate the covariance matrix of standardized data.</li>
    </ul>
    
    <h3>4. Eigen Decomposition</h3>
    <ul>
        <li>Compute eigenvalues and eigenvectors.</li>
        <li>Sort eigenvalues in descending order and arrange eigenvectors accordingly.</li>
    </ul>
    
    <h3>5. Dimensionality Reduction</h3>
    <ul>
        <li>Select the top <code>num_components</code> (default is 2) eigenvectors.</li>
        <li>Project data onto the selected principal components.</li>
    </ul>
    
    <h3>6. Visualization</h3>
    <ul>
        <li>Plot the original data (first two features) and the reduced data (first two principal components) using Matplotlib.</li>
    </ul>
    
    <h2>Output</h2>
    <ul>
        <li>The shape of the reduced data is printed.</li>
        <li>The first 5 rows of transformed data are displayed.</li>
        <li>Two scatter plots show a comparison between the original data and the PCA-transformed data.</li>
    </ul>
    
    <h2>Running the Script</h2>
    <p>Run the script using:</p>
    <pre><code>python pca_analysis.py</code></pre>
    <p>Ensure that <code>fuel_econ-2.csv</code> is in the correct directory.</p>
    
    <h2>Example Output</h2>
    <pre><code>Reduced Data Shape: (num_samples, 2)
First 5 rows of the reduced data:
[[value1, value2]
 [value3, value4]
 ...]</code></pre>
    
    <h2>Notes</h2>
    <ul>
        <li>PCA helps in reducing the dataset’s dimensions while retaining most of its variance.</li>
        <li>The number of principal components can be adjusted as needed.</li>
        <li>Ensure the dataset contains numerical values to avoid processing errors.</li>
    </ul>
    
    <h2>License</h2>
    <p>This project is open-source and available for educational purposes.</p>
</body>
</html>
