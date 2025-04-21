# Yeast-Protein-Clustering
This is a course project aimed at devising an unsupervised machine learning model to cluster the yeast protein data.

# Course : EE708 ( Even semester 2024-25 ). Intructor : Prof. Rajesh M. Hegde
Team Members : Myself (Suryansh Dwivedi, BT-BSBE Y22 Batch), Ganesh Srivathshava Burri (BS-Maths, Y22 Batch), Bhavnoor Singh(BT-CSE, Y23 Batch), Devansh(BT-CSE, Y23 Batch) and Ayushi Mishra(BT-BSBE, Y23 Batch).

**Aim**       : We are required to make a clustering algorithm based on yeast data provided by the 
                course intructor.

**Approach**  : We chose K-means clustering as the model that we will be applying on to cluster the data.
                It was the only ML model known to us that can be used for clustering the data at that point of time.

**Model**     : K-means clusterring involves specifying the number of clusters and specifying the distance metric,
                which will be used to form clusters by the model. The final aim was to arrive at the optimum number
                of clusters and an appropriate distance metric to form the best clusters possible

1. Obtaining the optimum number of clusters.

--> To arrive at the optimum number of clusters we initially used elbow method to find the point where there was 
a sharp dip in the intertia of the points. However, there was no such "elbow" in the plot of 
intertia vs number of clusters.
--> We then used Clustering Evaluation metrics, which are : Silhouette Scores, Davis-Bouldin score and Calinski Harabasz index
to evluate our clustering based on different number of clusters.
--> Upon plotting various plots of evaluating scores with the number of clusters we arrived at the optimum
number of clusters. It was 7 clusters.

2. Obtaining the perfect distance metric.
--> There are different distance metrics such as - Euclidean distance, Manhattan distance, Mahalonobis distance, etc.
--> 5 distance metrics were compared for the cluster being 7 based on the evauation scores. Euclidean gave the best scores
   out of all the distance metrics.

So, using the number of clusters being 7 and the distance metric being euclidean, we finally clustered the data.


# Limitation
1. One of the biggest limitation of our Project was not doing PCA (Principle component analysis), this would have
   given us a few and important features for the clustering process.
2. We didn't consider clustering algorithm apart from the K-means clustering. K-means form spherical clusters
   which may not always be how the data is spread in the n-dimensional space. At the time, we were only taught
   about the K-means which is why we could not explore any further.
                
