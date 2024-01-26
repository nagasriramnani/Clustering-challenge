# Clustering Challenge Project ML Intern Test 2024

## Overview
This repository contains the code and documentation for a clustering challenge involving a dataset of URLs, textual content, and high-dimensional embedding vectors. The objective of this project is to explore and understand the inherent groupings within the dataset using unsupervised machine learning techniques.

## Approach to solve this challenge: 

1. **Load the dataset** :from the provided daset.parquet file to examine its structure and contents.


2. **Data Preprocessing:** Ensure that the numerical data is in the correct format for analysis, handling any missing or malformed data.


3. **Exploratory Data Analysis (EDA):** Perform EDA to understand the distribution of the data and possibly reduce dimensionality for visualization.


4. **Clustering:** Apply unsupervised machine learning algorithms like K-means, DBSCAN, or hierarchical clustering to segment the data.


5. **Evaluation:** Evaluate the clusters using metrics like silhouette score or Davies-Bouldin index to assess the performance of the algorithm.


6. **Interpretation:** Use the URL and text contents as supplementary information to understand the context of the clusters formed.


7. **Further Steps:** Based on the initial findings, decide on further steps to refine the model, such as feature engineering, using different 
algorithms, or incorporating the supplementary data into the model in some form.



## Project Structure
The project is organized as follows:

- `data/`: Directory containing the dataset files, including the original `dataset.csv` and `dataset.parquet`, as well as cluster-specific data files.
- Generated sample clsuter files which are generated from the Step-6
- To run the code there is a file named MachineLearning_test.ipynb
- Make sure install all the Libraries requried

## Key Steps and Methodology
The project includes the following key steps and methodologies:

1. **Data Loading and Preprocessing**: The dataset was loaded from `dataset.parquet`, and data preprocessing steps were applied to handle missing values and ensure data consistency.

2. **Dimensionality Reduction**: Incremental PCA was used to reduce the dimensionality of the high-dimensional embedding vectors while retaining meaningful information.

3. **Text Vectorization**: PCA & TF-IDF vectorization was applied to the textual contents of the URLs to convert text into numerical data.

4. **Clustering**: Mini-Batch K-Means clustering was employed to group similar URLs together based on the reduced data.

5. **Evaluation**: The silhouette score was used as an evaluation metric to assess the quality of the clustering results.

6. **Visualization**: UMAP was used for dimensionality reduction and visualization to gain insights into the cluster structure.

## Results
- The clustering experiments resulted in moderate cluster separation, as indicated by the silhouette score.
- Visualizations generated using UMAP provided a 2D representation of the data, offering insights into the clustering effectiveness.

## Future Work
- Further more parameter tuning and experimentation with alternative clustering algorithms could potentially improve cluster quality.
- Exploring advanced text vectorization techniques and feature engineering may enhance clustering results.



