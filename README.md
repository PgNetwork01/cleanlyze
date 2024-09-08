# Cleanlyze

**Cleanlyze** is a Python library designed to streamline data processing tasks. With Cleanlyze, you can efficiently clean, transform, and visualize your data using powerful tools like `pandas`, `numpy`, and `scikit-learn`.

## Features

- **Data Cleaning**: Handle missing values, remove duplicates, and manage outliers with ease.
- **Data Transformation**: Normalize, scale, encode data, and create polynomial features for better machine learning models.
- **Visualization**: Create plots for data distribution, histograms, and correlation matrices.
- **File I/O**: Seamlessly read and write data from CSV, Excel, and other file formats.

## Commands

- remove_duplicates: 'Remove duplicate rows from DataFrame.',
- handle_missing_values: 'Handle missing values with specified strategy.',
- normalize_data: 'Normalize the DataFrame using Min-Max scaling.',
- create_polynomial_features: 'Create polynomial features of a specified degree.',
- plot_histogram: 'Plot a histogram for a specific column.',
- plot_correlation_matrix: 'Plot the correlation matrix of the DataFrame.',
- read_csv: 'Read a CSV file into a DataFrame.',
- write_csv: 'Write the DataFrame to a CSV file.'

## Installation

To install Cleanlyze, simply run:

```bash
pip install cleanlyze
```

## Example

```py
import cleanlyze as cz
import pandas as pd

# Load your data
df = pd.read_csv('data.csv')

# Clean the data by removing duplicates and handling missing values
df_cleaned = cz.cleaning.remove_duplicates(df)
df_cleaned = cz.cleaning.handle_missing_values(df_cleaned)

# Normalize the data
df_normalized = cz.transformation.normalize_data(df_cleaned)

# Plot the distribution of a column
cz.visualization.plot_histogram(df_normalized, 'column_name')
```
## Dependencies

- **Cleanlyze requires the following libraries:**

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- scipy

These will be installed automatically when you install Cleanlyze.

- **Contributing**

Contributions are welcome! If you'd like to contribute, please fork the repository and submit a pull request.

- **License**
This project is licensed under the MIT License.
