# unsupervised-machine-learning-challenge
Module 20 Challenge

# Description
Unsupervised learning is machine learning technique using algorithms to analyze and cluster unlabeled data. In contrast to supervised learning, unsupervised learning infers patterns within datasets without reference to known outcomes. It is compared to the human brain learning and searching for the underlying structure in the data. Unsupervised learning deals with two types of problems: clustering and association. Clustering searches and groups objects on commonalities and the lack thereof. Association is used for finding relationships between varabiles in the large dataset.

While there are many approaches and algorithms pertaining to unsupervised learning, this challenge primarily deals with principal component analysis and K-means clustering to build a model that can predict myopia in patients. Principal component analysis is a technique to limit dimensionality of a dataset. K-means clustering is a distance-based algorithm that assigns data points and measures the distance to centroids. This challenge also employs t-distributed stochastic neighbor embedding (t-SNE) to reduce and visualize the dataset dimensions.

In this repository, there is a Resources folder containing myopia data and a Jupyter notebook that walks through the steps of building an unsupervised learning model. 

Below is a summary of the steps to achieve the model:
1. Prepare and preprocess the data checking for null and duplicated values as well as scaling the data.
2. Apply dimensionality reduction with principal component analysis and t-SNE.
3. Perform a cluster anaylsis with K-means.


# Conclusions
After performing dimensionality reduction with PCA, the number of features reduced from 14 to 10. Running t-SNE on the output of PCA, the number of features reduced down to 2. But upon visualizing the t-SNE output, there are no distinct clusters. Using K-means for cluster analysis, the elbow curve points to possibly 3 clusterings of patients. Considering the size of the dataset, I would recommend exploring other cluster models, such as hierarchical clustering which works well with smaller datasets. Another recommendation is collecting more samples to the train the models.
