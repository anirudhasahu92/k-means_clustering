# Facebook Live Sellers in Thailand - K-Means Clustering Analysis

## Dataset Summary

The 'Facebook Live Sellers in Thailand' dataset from the UCI Machine Learning Repository contains information about live selling activities on the Facebook platform. It comprises 7050 observations and twelve attributes, including details about the time live sales are published and user engagements like sharing and reactions.

## Problem Statement

The aim is to analyze the dataset using K-Means clustering to identify groups of status types with similar behaviors. Status types can be videos, photos, statuses, and links, offering a detailed understanding of user engagement patterns.

## Steps Used

1. **Data Loading and Preprocessing:**
    - Load the dataset from the UCI repository into a pandas DataFrame.
    - Handle missing values and remove unnecessary columns.
2. **Data Transformation:**
    - Encode categorical features using label encoding.
    - Standardize the data using StandardScaler for better K-Means performance.
3. **Determining the Optimal Number of Clusters:**
    - Utilize the Elbow method to evaluate the within-cluster sum of squared distances (WCSS).
    - Employ the Silhouette method to assess the quality of clusters based on silhouette scores.
4. **K-Means Clustering:**
    - Create a K-Means model with the optimal number of clusters determined in the previous step.
    - Assign cluster labels to each data point.
5. **Visualization and Interpretation:**
    - Visualize the clusters using scatter plots for 2-dimensional representation.
    - Analyze the characteristics of each cluster to understand the patterns and behavior of different user engagement types.

## Libraries Used

- **numpy:** For numerical operations.
- **pandas:** For data manipulation.
- **matplotlib.pyplot:** For data visualization.
- **seaborn:** For statistical data visualization.
- **sklearn.preprocessing:** For data preprocessing techniques like label encoding and standardization.
- **sklearn.cluster:** For implementing the K-Means clustering algorithm.
- **sklearn.metrics:** For evaluating clustering quality using silhouette scores.


## Acknowledgement

This analysis utilizes the 'Facebook Live Sellers in Thailand' dataset sourced from the UCI Machine Learning Repository.


