# Linear_Regression  &   K-Nearest & K-Means Clustering

term regression is used when you try to find the relationship between variables.

Linear regression uses the relationship between the data-points to draw a straight line through all them.
#This line can be used to predict future values.

************************************************************************************

K-Nearest Neighbor(KNN) Algorithm for Machine Learning

    K-Nearest Neighbour is one of the simplest Machine Learning algorithms based on Supervised Learning technique.
    K-NN algorithm assumes the similarity between the new case/data and available cases and put the new case into the category that is most similar to the available categories.
    K-NN algorithm stores all the available data and classifies a new data point based on the similarity. This means when new data appears then it can be easily classified into a well suite category by using K- NN algorithm.
    K-NN algorithm can be used for Regression as well as for Classification but mostly it is used for the Classification problems.
    K-NN is a non-parametric algorithm, which means it does not make any assumption on underlying data.
    It is also called a lazy learner algorithm because it does not learn from the training set immediately instead it stores the dataset and at the time of classification, it performs an action on the dataset.
    KNN algorithm at the training phase just stores the dataset and when it gets new data, then it classifies that data into a category that is much similar to the new data.
    Example: Suppose, we have an image of a creature that looks similar to cat and dog, but we want to know either it is a cat or dog. So for this identification, we can use the KNN algorithm, as it works on a similarity measure. Our KNN model will find the similar features of the new data set to the cats and dogs images and based on the most similar features it will put it in either cat or dog category.

************************************************************************************
K-Means Clustering Explained

Clustering was introduced in 1932 by H.E. Driver and A.L.Kroeber in their paper on “Quantitative expression of cultural relationship”. Since then this technique has taken a big leap and has been used to discover the unknown in a number of application areas eg. Healthcare. Clustering is a type of unsupervised learning where the references need to be drawn from unlabelled datasets. Generally, it is used to capture meaningful structure, underlying processes, and grouping inherent in a dataset. In clustering, the task is to divide the population into several groups in such a way that the data points in the same groups are more similar to each other than the data points in other groups. In short, it is a collection of objects based on their similarities and dissimilarities. With clustering, data scientists can discover intrinsic grouping among unlabelled data. Though there are no specific criteria for a good clustering and it completely depends on the user, how they want to use it for their specific needs. It can be used to find unusual data points/outliers in the data or to identify unknown properties to find a suitable grouping in the dataset. Let’s take an example, imagine you work in a Walmart Store as a manager and would like to better understand your customers to scale up your business by using new and improved marketing strategies. It is difficult to segment your customers manually. You have some data that contains their age and purchase history, here clustering can help to group customers based on their spending. Once the customer segmentation will be done, you can define different marketing strategies for each of the groups as per target audiences. There are many clustering algorithms grouped into different cluster models. Before choosing any algorithm for a use case, it is important to get familiar with the cluster models and if it is suitable for the use case. One more thing which should be considered while choosing any clustering algorithm is the size of your dataset. Datasets can contain millions of records and not all algorithms scale efficiently. K-Means is one of the most popular algorithms and it is also scale-efficient as it has a complexity of O(n). In this article, we will talk about K-Means in-depth and what makes it popular.
How does K-means work?
1.	Choosing the number of clusters
 The first step is to define the K number of clusters in which we will group the data. Let’s select K=3.



2.	Initializing centroids
Centroid is the center of a cluster but initially, the exact center of data points will be unknown so, we select random data points and define them as centroids for each cluster. We will initialize 3 centroids in the dataset.
3.	Assign data points to the nearest cluster
Now that centroids are initialized, the next step is to assign data points Xn to their closest cluster centroid Ck
In this step, we will first calculate the distance between data point X and centroid C using Euclidean Distance metric.
And then choose the cluster for data points where the distance between the data point and the centroid is minimum. 
4.	Repeat steps 3 and 4
We will keep repeating steps 3 and 4 until we have optimal centroids and the assignments of data points to correct clusters are not changing anymore.
Does this iterative process sound familiar? Well, K-means follows the same approach as Expectation-Maximization(EM). EM is an iterative method to find the maximum likelihood of parameters where the machine learning model depends on unobserved features. This approach consists of two steps Expectation(E) and Maximization(M) and iterates between these two. For K-means, The Expectation(E) step is where each data point is assigned to the most likely cluster and the Maximization(M) step is where the centroids are recomputed using the least square optimization technique.
