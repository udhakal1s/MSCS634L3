# Name: Umesh Dhakal
# Course: MSCS634
# Professor: Dr. Satish Penmatsa
# February 13, 2026
# Lab 3- Clustering Analysis Using K-Means and K-Medoids Algorithms

## Purpose of the Lab
The purpose of this lab is to understand how clustering algorithms work on real data.In this lab, we use the Wine dataset from scikit-learn to apply and compare two unsupervised learning methods: K-Means and K-Medoids. The goal is to see how well these algorithms group similar data points and how closely the clusters match the actual wine classes.

## Key Insights and Observations
Based on the clustering results, both K-Means and K-Medoids were able to group the Wine dataset into three clusters, which matches the actual number of wine classes in the dataset. Comparing the the silhouette scores, K-Means produced slightly tighter clusters overall. This shows that the data points inside each cluster were more closely grouped together, which means the cluster boundaries were more clearly define. The Adjusted Rand Index  also showed that K-Means had a slightly better match with the real class labels compared to K-Medoids, even though both methods performed reasonably well.
One of the difference I notice between the two algorithms was how the cluster centers were handled. K-Means uses the mean of the data points as the cluster center which makes it efficient and effective when the data is evenly distributed. However, this also means it can be sensitive to extreme values. On the other hand, K-Medoids selects actual data points as the cluster centers which makes it more stable and less affected by potential outliers. Because of this, the K-Medoids clusters appeared slightly more spread out, but also more realistic in terms of representing actual data samples. K-Means performed slightly better for this dataset because the Wine data is well-structured and does not contain extreme outliers. K-Medoids still provided meaningful clusters and demonstrated its advantage in robustness. 

## Challenges
The challenge I faced during the lab was installing external libraries for K-Medoids on a Windows environment. To avoid installation issues, I implemented K-Medoids manually using a PAM-style approach.


