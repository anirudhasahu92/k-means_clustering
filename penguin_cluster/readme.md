# Penguin Clustering Analysis

This project analyzes a dataset of penguins to identify clusters based on their physical characteristics and sex. 

## Data and Features

The dataset contains the following features:

* **culmen_length_mm:** Culmen length (mm)
* **culmen_depth_mm:** Culmen depth (mm)
* **flipper_length_mm:** Flipper length (mm)
* **body_mass_g:** Body mass (g)
* **sex:** Penguin sex

## Methodology

1. **Data Preprocessing:** 
   - Handling missing values by dropping rows with null values.
   - Identifying and treating outliers.
   - Creating dummy variables for the 'sex' feature to enable clustering.

2. **Feature Scaling:**
   - Standardizing features using StandardScaler to ensure that all features contribute equally to the analysis.

3. **Dimensionality Reduction (PCA):**
   - Applying Principal Component Analysis (PCA) to reduce the dimensionality of the data while retaining a significant portion of the information.
   - Using 85% variance explained to select the optimal number of principal components.

4. **Determining the Number of Clusters (Elbow Method):**
   - Implementing the Elbow method to determine the optimal number of clusters for K-Means clustering.
   - Plotting the within-cluster sum of squares (WCSS) for different numbers of clusters.
   - Observing the elbow point in the plot to identify the appropriate number of clusters.

5. **K-Means Clustering:**
   - Applying K-Means clustering with the identified number of clusters (4 in this case).
   - Assigning cluster labels to each penguin observation.

6. **Visualization:**
   - Creating a scatter plot using the first two principal components to visualize the clusters.
   - Utilizing Plotly for interactive exploration of the clusters.

## Results

The analysis resulted in the identification of four distinct penguin clusters. Visualizations based on the principal components clearly show the separation of these clusters.

## Future Work

* Further investigate the characteristics of each cluster through exploratory data analysis.
* Explore other clustering algorithms like hierarchical clustering.
* Develop a classification model to predict the cluster of a new penguin based on its physical characteristics.
