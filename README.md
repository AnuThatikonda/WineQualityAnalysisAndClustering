# Wine Quality Analysis and Clustering

## Project Description

This project conducts a comprehensive analysis of red and white wines by leveraging clustering techniques and Self-Organizing Maps (SOM). The objective is to explore the differences between the two types of wines, identify key attributes, and understand the underlying patterns in the dataset.

## Data Source

The datasets used in this analysis are sourced from the UCI Machine Learning Repository:
- [Red Wine Quality Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv)
- [White Wine Quality Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-white.csv)

## Project Workflow

### 1. Data Preparation and Cleaning
- Load red and white wine datasets.
- Combine the datasets and add a `wine_type` attribute to distinguish between red and white wines.
- Verify there are no missing values and examine the data structure.

### 2. Exploratory Data Analysis
- Create box plots and histograms to visualize the distribution of quality, alcohol content, and pH levels.
- Conduct correlation analysis and generate a heatmap to explore relationships between different chemical properties.

### 3. Dimensionality Reduction and Clustering
- Apply Principal Component Analysis (PCA) to reduce the dimensionality of the dataset.
- Determine the optimal number of clusters using silhouette analysis and perform K-means clustering on the principal components.
- Visualize the clusters using a score plot colored by wine type.

### 4. Self-Organizing Maps (SOM)
- Fit a SOM to the scaled wine data to capture the high-dimensional structure in a low-dimensional grid.
- Visualize the SOM mapping to identify clusters and patterns related to wine types.
- Perform hierarchical clustering on the SOM codebook vectors to analyze the learned prototypes.

### 5. Component Plane Plots
- Generate component plane plots for each attribute to visualize the distribution of values across the SOM grid and identify significant patterns.

## Summary of Findings
- Key differences in the chemical properties of red and white wines, such as higher alcohol content and pH levels in white wines.
- PCA and K-means clustering identified four well-separated clusters, indicating distinct groups within the dataset.
- SOM visualization provided an intuitive understanding of the relationships between different wine attributes and helped uncover hierarchical structures in the data.

## Technologies and Libraries Used
- **R Programming Language**
- **Libraries:** dplyr, ggplot2, FactoMineR, factoextra, kohonen, cluster

## Conclusion
- This project demonstrates the application of advanced data analysis techniques, including PCA, K-means clustering, and SOM, to uncover patterns and insights in wine datasets. The findings highlight the chemical differences between red and white wines and provide a framework for further exploration and analysis.

