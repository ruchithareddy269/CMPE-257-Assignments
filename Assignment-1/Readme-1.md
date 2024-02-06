##House Price Prediction:
This project aims to predict house prices using a dataset containing various features such as location coordinates, housing age, total rooms, median income, and more. The project involves data wrangling, preparation, and clustering techniques to gain insights and potentially improve prediction accuracy.

##Dataset Wrangling
The dataset used in this project is sourced from the California Housing Prices dataset available on Kaggle. It contains various attributes such as longitude, latitude, housing median age, total rooms, total bedrooms, population, households, median income, median house value, and ocean proximity. The following steps are involved in data wrangling:

###Loading the Dataset: The dataset is loaded from the CSV file using pandas.

###Basic Statistics and Information: Basic statistical measures and information about the dataset are displayed using describe() and info() functions.

###Handling Missing Values: Any missing values in the dataset, typically in the total_bedrooms column, are handled by dropping the corresponding rows using the dropna() function.

###Encoding Categorical Feature: The categorical feature ocean_proximity is encoded using one-hot encoding to convert it into numerical format suitable for machine learning algorithms.

###Dataset Preparation
After data wrangling, the dataset is prepared for clustering and subsequent analysis. This involves the following steps:

###Feature Selection: Relevant features for clustering and prediction are selected based on their importance and correlation with the target variable.

###Normalization: Numeric features are normalized to ensure that they are on a similar scale, preventing certain features from dominating the clustering process.

###Splitting the Dataset: The dataset is split into training and testing sets to evaluate the performance of the clustering algorithm.

##Clustering
Clustering is performed on the prepared dataset to identify patterns and group similar data points together. In this project, K-means clustering and Gaussian Mixture Model (GMM) clustering are applied:

###K-means Clustering: K-means clustering is a popular unsupervised learning algorithm that partitions the dataset into K clusters. The following steps are involved:
Choose the number of clusters (K).
Apply K-means clustering using the KMeans class from scikit-learn.
Visualize the clusters using scatter plots.


###Gaussian Mixture Model (GMM) Clustering: GMM clustering is a probabilistic model that assumes that the data points are generated from a mixture of several Gaussian distributions. The steps include:

Choose the number of components (clusters) for the GMM.
Apply GMM clustering using the GaussianMixture class from scikit-learn.
Visualize the clusters using scatter plots.
