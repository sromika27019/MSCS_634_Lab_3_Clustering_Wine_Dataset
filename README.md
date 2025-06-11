# MSCS_634_Lab_3_Clustering_Wine_Dataset

# MSCS_634_Lab_3: Clustering with K-Means and K-Medoids

## Purpose of the Lab

The purpose of this lab is to explore and compare two clustering techniques—**K-Means** and **K-Medoids**—using the **Wine Dataset** from the sklearn Python library. The task involves clustering the dataset, evaluating the clustering performance using the **Silhouette Score** and **Adjusted Rand Index (ARI)**, and visualizing the clustering results.

## Key Insights from the Clustering Results

- **K-Means Clustering:**  
  K-Means clustering assigns data points to the nearest centroid and is sensitive to the initial selection of centroids. The centroids are updated iteratively to minimize the sum of squared distances from each point to its assigned centroid. The K-Means algorithm performed well in terms of cluster cohesion, as evidenced by the silhouette score.

- **K-Medoids Clustering:**  
  Unlike K-Means, K-Medoids chooses actual data points as cluster centers (medoids), making it more robust to outliers. In this lab, we observed that K-Medoids produced more distinct clusters for certain points, especially in the presence of outliers. The algorithm's performance was also evaluated using the same metrics as K-Means.

- **Cluster Visualization:**  
  The visualizations show the differences between the two clustering techniques. In the K-Means plot, the centroids (marked with red crosses) seem to be in the center of each cluster, while K-Medoids places the red crosses on actual data points. Both methods show similar overall clustering behavior, but K-Medoids' handling of outliers was slightly better in some cases.

## Key Challenges Faced

- **Choosing the Right Number of Clusters:**  
  The lab specifies **k=3**, as the Wine dataset has three classes. In practice, selecting the correct number of clusters can be challenging and may require techniques like the **Elbow Method** or **Silhouette Analysis**.

- **Data Preprocessing:**  
  Ensuring that the data is standardized before applying clustering algorithms is crucial, as both K-Means and K-Medoids are sensitive to the scale of the data. Using **Z-score normalization** helped standardize the data.

## Instructions for Running the Code

1. **Install Required Libraries:**
   Ensure you have the necessary libraries installed:
   ```bash
   pip install scikit-learn pyclustering matplotlib
Running the Code:

Download or clone this repository to your local machine.

Open the Jupyter Notebook MSCS_634_Lab_3_Clustering_Wine_Dataset.ipynb.

Execute the code cells step by step to load the dataset, apply the clustering algorithms, and visualize the results.

Results and Visualizations
K-Means Clustering:
The first plot shows the results of K-Means clustering. Each data point is colored based on its assigned cluster, and the red crosses represent the centroids of the clusters.

K-Medoids Clustering:
The second plot shows the results of K-Medoids clustering. Similar to K-Means, the data points are colored according to their cluster, but the red crosses represent actual data points (medoids) instead of centroids.

Conclusion
Both K-Means and K-Medoids provide effective clustering results, but K-Medoids is more robust to outliers as it uses actual data points as the centers.

K-Means is more sensitive to initialization and can lead to suboptimal clustering if the initial centroids are poorly chosen.

Future Work
Explore other clustering algorithms such as DBSCAN or Agglomerative Clustering.

Experiment with different initialization methods for K-Means (e.g., k-means++).

Perform hyperparameter tuning for K-Medoids to evaluate its performance with different initial medoids.

License
This project is licensed under the MIT License - see the LICENSE file for details.



### Instructions for Customizing:
1. **Purpose of the Lab** - Provides an overview of what the lab is about and what algorithms you used.
2. **Key Insights** - A section to summarize your findings and results, especially focusing on the differences between K-Means and K-Medoids.
3. **Key Challenges Faced** - Acknowledge any difficulties or challenges you encountered during the lab.
4. **Instructions for Running the Code** - Gives details on setting up the environment and running the code.
5. **Results and Visualizations** - Provides an explanation of the results and how to interpret the visualizations.
6. **Conclusion** - Summarizes the takeaways from the lab and any differences you observed between the two clustering techniques.
7. **Future Work** - Suggest areas for improvement or additional work that could be done based on the lab findings.
