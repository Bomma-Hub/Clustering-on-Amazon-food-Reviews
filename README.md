# Clustering-on-Amazon-food-Reviews
Implementation of clustering techniques on Amazon food reviews
Clustering Methodologies: 
We try to find homogeneous subgroups within the data such that data points in each cluster are as similar as possible according to a similarity measure such as euclidean-based distance or correlation-based distance. The decision of which similarity measure to use is application-specific

K-Means Clustering
1)	K-Means is a centroid based clustering.
2)	Kmeans algorithm is an iterative algorithm that tries to partition the dataset into Kpre-defined distinct non-overlapping subgroups (clusters) where each data point belongs to only one group.
3)	Kmeans algorithm is an iterative algorithm that tries to partition the dataset into Kpre-defined distinct non-overlapping subgroups (clusters) where each data point belongs to only one group.
4)	It assigns data points to a cluster such that the sum of the squared distance between the data points and the cluster’s centroid (arithmetic mean of all the data points that belong to that cluster) is at the minimum. 
5)	In K-Means , ‘K’ is hyperparameter i.e it represents how many clusters to be made with the dataset.
 

6)	In K-means we get K-centroids and K-sets.
7)	Where centroid is mean(geometrically ) of all the points in the set.
 

Steps to find centroids and clusters:
a.	In this methodology, We calculate distance between each and every centroid to every point in dataset.
b.	Then we map all the points to the centroid which has shortest distance from it
c.	Find the centroid such that each of the point is assigned to its nearest centroid the intra cluster distance is minimized.

Lloyd’s Algorithm:
•	Initialization: Randomly select k points and make them as k-centroids.
•	For each point in dataset , select nearest centroid  “cj” and add the point to set “sj”.
•	Recalculate Cj’s i.e calculating the mean point from respective sets
 			 
•	Repeating step 2 and 3 until converge (i.e centroids don’t change much)






Agglomerative Clustering
Agglomerative : Grouping
How it works:
•	Initially It assumes each point as a cluster
•	Then it combines two nearest clusters as one cluster.
•	It keeps on repeating this process until single cluster is reached.
 
Divisive: It works quite opposite to the agglomerative clustering.
It does the same process from bottom u approach.
i.e It assumes it assumes entire datapoints as one cluster. Then it keeps on dividing the cluster into multiple clusters till single datapoint cluster has achieved
 

Dendogram: It is tree which records the sequence of merges (Agglomerative )or splits(Divisive)

Key Point: In agglomerative clustering, we can get the different number clusters without retraining the model which is not in the case of K-means, as in K-means we need to retrain the model if we are not happy with results of k-clusters (k = any number)

 
 


 

  

Reference link: https://cs.wmich.edu/alfuqaha/summer14/cs6530/lectures/ClusteringAnalysis.pdf  
DBSCAN  (Density Base Spatial Clustering of Applications with Noise)

https://github.com/PushpendraSinghChauhan/Amazon-Fine-Food-Reviews/blob/master/Apply%20DBSCAN%20on%20Amazon%20Fine%20Food%20Reviews.ipynb

