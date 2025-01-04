# Principal Component Analysis and Clustering

This project demonstrates how to apply **Principal Component Analysis (PCA)** for dimensionality reduction and perform **clustering** using the first three principal component scores. Both **hierarchical clustering** and **K-means clustering** are used to determine the optimal number of clusters, and the results are validated against the original data.  

---

## Table of Contents
- [Introduction](#introduction)
- [Project Workflow](#project-workflow)
- [Results and Validation](#results-and-validation)
- [Visualizations](#visualizations)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)

---

## Introduction
Principal Component Analysis is applied to reduce high-dimensional data into fewer dimensions (principal components). Using these principal components:
1. Perform **clustering** to group similar data points.
2. Determine the **optimal number of clusters** using techniques such as the scree plot and elbow curve.
3. Validate the clustering results with the original data (ignoring the `class` column initially).

---

## Project Workflow
1. **Data Preprocessing**:
   - Scale the data using `StandardScaler`.
   - Apply PCA to extract principal component scores.
2. **Clustering**:
   - Perform hierarchical clustering on the first three principal components.
   - Use K-means clustering to analyze the same.
3. **Determine Optimal Clusters**:
   - Generate a scree plot for PCA.
   - Use an elbow curve to find the optimal number of clusters.
4. **Validation**:
   - Compare clustering results with the original dataset's class column.
5. **Visualization**:
   - Plot dendrograms, elbow curves, and scatter plots for better understanding.

---

## Results and Validation
- Using the first 3 principal components, we identified clusters that closely match the original dataset's clusters.
- The optimal number of clusters is determined using the elbow method and scree plot.
- Results are validated with the original data's class column, confirming consistency.

---

## Visualizations
1. **Scree Plot**: To analyze the variance explained by each principal component.
2. **Elbow Curve**: To find the optimal number of clusters for K-means.
3. **Dendrogram**: For hierarchical clustering visualization.
4. **Cluster Scatter Plot**: To visualize clustering results in 2D/3D.

---

## Technologies Used
- **Python**: Programming language.
- **Libraries**: 
  - `pandas` and `numpy`: Data manipulation.
  - `scikit-learn`: PCA, K-means clustering, scaling.
  - `matplotlib` and `seaborn`: Visualization.

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/R-Mahesh45/pca-clustering.git
   cd pca-clustering
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage
1. Run the script to perform PCA and clustering:
   ```bash
   python pca_clustering.py
   ```
2. Modify clustering parameters, such as the number of clusters, in the code for experiments.
3. View visualizations for analysis.

---

## Future Enhancements
- Extend the clustering to more datasets.
- Automate optimal cluster detection using silhouette scores.
- Add interactive visualizations using Plotly or Dash.

---

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request for improvements.
