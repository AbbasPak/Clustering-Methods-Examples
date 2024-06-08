## Gaussian Mixture Models

A Gaussian Mixture Model (GMM) is a probabilistic model that assumes all the data points are generated from a mixture of several Gaussian distributions with unknown parameters. It is widely used in clustering, where the goal is to partition a dataset into subgroups, such that data points in the same group are more similar to each other than to those in other groups. 


While k-means clustering is a popular and straightforward algorithm for clustering, it has several drawbacks:
1. Assumption of Spherical Clusters: K-means: Assumes that clusters are spherical (or roughly spherical) and of similar size. This means it doesn't perform well on clusters with different shapes and sizes.
2. Hard Assignments: K-means: Assigns each data point to exactly one cluster (hard clustering), which can be too restrictive and lead to misclassification, especially when data points are near the boundary of clusters.
3. Cluster Overlap: K-means: Struggles with overlapping clusters because it assigns each point to the closest centroid, which might not be meaningful if clusters overlap.
4. Handling of Outliers: K-means: Can be significantly affected by outliers, as they can distort the mean position of clusters.

    



    







#### Advantages

•	Flexibility: GMM can model clusters of different shapes and sizes because each cluster is represented by its own Gaussian distribution with its own mean and covariance.

•	Soft Clustering: Provides probabilistic cluster memberships, which can be more informative than hard assignments.

#### Limitations:

•	Computational Complexity: EM algorithm can be computationally intensive, especially for large datasets or high-dimensional data.
•	Local Optima: EM algorithm can converge to local optima, depending on the initialization. Multiple runs with different initializations are often used to mitigate this.
•	Assumption of Gaussian Distribution: The model assumes that the data within each cluster follow a Gaussian distribution, which may not always be true.

#### Applications

•	Image and Speech Recognition: GMMs are used to model the distribution of features in image and speech data.
•	Anomaly Detection: By modeling normal data with GMMs, anomalies can be detected as data points with low likelihood under the model.
•	Finance: Used for modeling and forecasting financial data distributions.



### References

1. https://www.javatpoint.com/k-means-clustering-algorithm-in-machine-learning
2. https://www.geeksforgeeks.org/dbscan-clustering-in-ml-density-based-clustering/
3. https://www.analyticsvidhya.com/blog/2020/09/how-dbscan-clustering-works/
4. Gareth James, Daniela Witten, Trevor Hastie, Robert Tibshirani, (2013). 
An introduction to statistical learning : with applications in R. New York :Springer.

