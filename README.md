
# K-Means Clustering with Outliers Removal

This Python script implements K-Means clustering algorithm with the option to remove outliers from the dataset before clustering. It provides a graphical user interface (GUI) built using Tkinter.

## Prerequisites
- Python 3.x
- Required Python libraries: tkinter, pandas, numpy

## How to Use
1. Run the script.
2. Select a CSV file containing the dataset using the "Browse" button.
3. Enter the percentage of data you want to consider and the number of clusters (K).
4. Click on the "Run K-Means with Outliers Removed" button.
5. The centroids, cluster sizes, outliers, and content of each cluster will be displayed in the GUI.

## Functions Overview
- `initialize_centroids(data, k)`: Initializes centroids randomly.
- `euclidean_distance(x1, x2)`: Calculates Euclidean distance between two points.
- `assign_clusters(data, centroids)`: Assigns data points to clusters based on nearest centroid.
- `update_centroids(data, clusters)`: Updates centroids based on mean of data points in each cluster.
- `kmeans(data, k, max_iters)`: Performs K-Means clustering.
- `browse_file()`: Opens a file dialog to browse and select a CSV file.
- `check_outliers(data, percentage)`: Identifies outliers in the dataset based on a given percentage.
- `run_kmeans_with_outliers()`: Runs K-Means clustering with outliers removed and displays results in the GUI.

## GUI Elements
- **File Selection**: Allows selecting a CSV file containing the dataset.
- **Percentage of Data**: Input field to specify the percentage of data to consider for clustering.
- **Number of Clusters (K)**: Input field to specify the number of clusters for K-Means.
- **Run Button**: Executes K-Means clustering with outliers removed.
- **Output Text Area**: Displays centroids, cluster sizes, outliers, and content of each cluster.

## Error Handling
- Displays error message in case of any exceptions during execution.

## Note
- Outliers are identified using the IQR (Interquartile Range) method.
- The GUI provides a user-friendly interface for selecting files and viewing results.
