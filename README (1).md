
# Netflix Movies & TV Shows Clustering

With the advent of streaming platforms, there’s no doubt that Netflix has become one of the important platforms for streaming. The dataset that we have used for EDA and clustering has been collected by Flixable, a third-party Netflix search engine. There are 12 features and around 7700 observations in the dataset and are mostly textual features.

Through univariate and multivariate analysis, we found trends that will help in understanding     what content is being consumed country-wise, depending on some categorical features like rating, type, genres, cast, directors, etc. Clustering was performed along with NLP on textual columns and then a mini-recommendation system was built out of it.

Keywords—Machine Learning, Explanatory Data Analysis, Netflix, TV Shows, Movies, Genre, Clustering, K Means.

## Introduction
Unsupervised Learning is a machine learning technique in which the models are not supervised by the training set instead we find hidden patterns and insights from the given data. It is a machine learning technique in which models are trained on the unlabeled data set without any supervision. 

A cluster is a collection of elements that are similar to each other but dissimilar to the elements belonging to other clusters. Clustering can be done using various kinds of distances such as Euclidean distance, Manhattan distance, gomer distance, etc. We can do different kinds of clustering based on the data pattern in space such as spherical clustering, K-means clustering, etc.


## Problem Statement

This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.
In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

In this project, you are required to do –

1. Exploratory Data Analysis.
2. Understanding what type content is available in different countries.
3. Is Netflix increasingly focused on TV rather than movies in recent
years?
4. Clustering similar content by matching text-based features

Our goal here is to make an unsupervised clustering model, which will help in garnering insights on Netflix and how its content is being consumed.

## Dataset
[Dataset from Flixable - A third-party Netflix search engine.](https://drive.google.com/file/d/12U7pvtOG9mVLNMGuc6hFyydI4Ya3_iJc/view?usp=sharing)

A brief summary of the dataset is given below:

Show id: Unique ID for every Movie / TV Show 
type – Identifier - A Movie or TV Show 
title – Title of the Movie / TV Show 
director-director of the content 
cast –Actors involved in the movie / show 
country – Country where the movie / show was produced 
date_added – Date it was added on Netflix 
release_year – Actual Release year of the movie / show 
rating – TV Rating of the movie / show 
duration – Total Duration - in minutes or number of seasons 
listed_in – genre 
description – The Summary description

## Algorithm Used
1.	K-means Clustering
k-means clustering is a method of vector quantization, originally from signal processing, that aims to partition n observations into k clusters in which each observation belongs to the cluster with the nearest mean (cluster centers or cluster centroid), serving as a prototype of the cluster.

We created the sample data using build blobs and used range_n_clusters to specify the number of clusters we wanted to utilize in k means.

2.	Heirarchial clustring
The number of clusters will be the number of vertical lines which are being intersected by the line drawn using the threshold .
So we consider, no. of Cluster = 3

3.	Agglomerative Clustering

The agglomerative clustering is the most common type of hierarchical clustering
used to group objects in clusters based on their similarity. Next, pairs of
clusters are successively merged until all clusters have been merged into one big cluster containing all objects.

## Conclusion
Following conclusion were drawn -

•	 We started by removing NaN values and converting the Netflix added date to year, month, and day using date time format.

•	Most films were released in the years 2018, 2019, and 2020.

•	The months of October, November, December and January had the largest number of films and television series released.

•	TV shows account for 2.8 percent of the total, while movies account for 97.2 percent.

•	The United States, India, the United Kingdom, Canada, and Egypt are the top five producer countries.

•	Netflix has added a lot more movies and TV episodes in the previous years, but the numbers are still low when compared to movies released in the last ten years.

•	We did feature engineering, which involved removing certain variables and preparing a dataframe to feed the clustering algorithms.

•	For the clustering algorithm, we utilized type, director, nation, released year, genre, and year.

•	Affinity Propagation, Agglomerative Clustering, and K-means Clustering were utilised to build the model.

•	In Affinity Propagation, we had 9 clusters and a Silhouette Coefficient score of 0.340.

•	A dendrogram was used to determine the number of clusters in Agglomerative Clustering. There were two clusters, with an average silhouette score of 0.56590662228136.

•	The final model we used was k-means clustering, which consisted of 2,3,4,5,6 clusters. 3 numbers of clusters gives us good fitting.

•	After clustering, we can say that the number of TV shows launched in the previous years is NOT growing.

•	The number of TV shows added to Netflix is higher in the last three years.


## Reference
1.  Applied Science Article  MDPI
2.  GeeksforGeeks
3.  Wikipedia
4.  DataCamp

## 🚀 About Me


- 👋 Hi, I’m Shahrukh, a curious Data Dcientist
- 👀 I’m currently working on Machine Learning projects.
- 🌱 I’m currently learning various machine learning models and deep learning techniques.
- 💞️ I’m would love to collaborate on Machine Learning projects.
- 📫 How to reach me : khan441shahrukh@gmail.com
- 👀 LinkedIn : https://www.linkedin.com/in/md-shahrukh-khan-49a027172/