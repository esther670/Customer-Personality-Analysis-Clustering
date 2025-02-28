# Customer-Personality-Analysis-Clustering
## Project Description
In this project, you will use a clustering algorithm to perform customer segmentation on a dataset. Customer segmentation is a common technique used in marketing to divide customers into groups based on similar characteristics, such as purchasing behavior or demographics. By segmenting customers, businesses can gain valuable insights to tailor their marketing strategies, product offerings, and customer service.

## Dataset
You can pick any relevant dataset. Choose a dataset that contains relevant features such as customer demographics (age, gender, location), transaction history (purchase amounts, frequency), and any other information that you think might be useful for customer segmentation. Ensure that the dataset is preprocessed and cleaned before applying the algorithm.

## Data Preprocessing
- Handled missing values by removing affected rows.
- Created a new feature `Age` from the year of birth.
- Standardized numerical features for clustering.

## Dimensionality Reduction
- Principal Component Analysis (PCA) was used to reduce the number of dimensions while retaining 95% essential variance.

## Perform clustering
The following clustering techniques were applied:
- K-Means Clustering: Groups customers into predefined clusters. By using the elbow method, I got the optimal number of clusters to use in the modelling.
- DBSCAN: Identifies density-based clusters.
- Agglomerative Clustering: Performs hierarchical clustering.
- Gaussian Mixture Models (GMM): Probabilistic clustering approach. Used aic and bic to predict the best number of components to use in modelling>

## Evaluation of the model performance
To assess clustering performance, the following metrics were used:
- Silhouette Score - Score ranges from -1 to 1 (higher values indicate better-defined clusters).
- Davies-Bouldin Score - Lower values indicate better clustering (as clusters are more distinct).
- Calinski-Harabasz Score

## Analysis and Interpretation of the model performance
- K-Means is the best overall performer when considering all three metrics. It has the highest Calinski-Harabasz Score, meaning the clusters are well-separated, and its Davies-Bouldin Index is relatively low.
- Hierarchical Clustering has some similarity to K-Means, slightly outperforming it in Silhouette Score but performing worse in the Calinski-Harabasz Score.
- GMM performs the worst in all three metrics, indicating that it struggles to define clear cluster boundaries.
- DBSCAN has the best Silhouette Score and Davies-Bouldin Index, meaning it finds well-defined and distinct clusters. However, its Calinski-Harabasz Score is very low.


## Make sure you perform cluster analysis and interpretation:

- Evaluate the quality of the clusters formed using appropriate metrics like the within-cluster sum of squares (WCSS) or silhouette score.
- Analyze and interpret the characteristics of each customer cluster, identifying meaningful patterns and insights.
- Visualize the clusters using scatterplots or other suitable visualization techniques to understand the separation.
- Remember to document your process, explain your decisions, and present your results effectively. Good luck with your project!





