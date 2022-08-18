# NetFlix Movies and Tv shows Clustering
# PROBLEM STATEMENT:
	The data is related to Netflix movies and tv shows till 2019. It is understandable from the data that tv shows number has been tripled from 2010 and the number of movie titles has been reduced by 2000. We have to find several insights from the data using EDA and also, have to cluster the data based on the data.

# INTRODUCTION:
In this project we have to perform the following
1.	Exploratory Data Analysis
2.	Understanding what type of content is available in different countries
3.	Is Netflix focusing more on tv shows rather on movies
4.	Cluster similar content by matching text data.

# STEPS INVOLVED:
1. Exploratory Data Analysis
2. Handling Null Values
3. Data Wrangling
4. Data Visualizations
5. Training and Fitting Model
6. Recommender System

# KMeans Clustering:
  It is an unsupervised learning algorithm that is used to solve the clustering problems in machine learning or data science. It groups the unlabeled dataset into different clusters. Here k defines the number of pre-defined clusters that need to be created in the process, as if k=2, there will be two clusters, and for k=3 there will be three clusters, and so on.
	The performance of k-means clustering depends upon highly efficient clusters that it forms. But choosing the optimal number of clusters is a big task. There are some different ways to find the optimal cluster size
1. Elbow method 
2. Silhouette Score
![image](https://user-images.githubusercontent.com/86276183/185300841-ce4fd48a-7b38-46d4-a1a6-c49000b82e37.png)

# Conclusion:
	After Implementing very good analysis and most of the visualisations we have a pretty good idea of what this dataset represents. Dataset contains 7787 Rows and 12 Columns, there are around 2800 null values in director column, 718 on cast and 507 in country.

The main content providers for Netflix are the United States which contributes 50% of the content, followed by India it contributes 14% and United Kingdom comes third of 8.5% and the rest follows.

This Netflix dataset has been categorised into two items:
•	Movies
•	TV Shows

Movies is the majority here which covers around 69% and TV Shows covers the rest which is 31% of the dataset.

In the Movies section 48% of the movies are Adult rated, 31% rated as Teen, 15.9% as 7&above, and the rest as Kids.

In the TV Shows section 41% of the shows are Adult rated, 27% rated as Teen, 20% as 7&above and the rest 10% as kids Rated.

The year 2017 saw the highest content ever on Netflix for movies where 744 movies were released and the yesr 2020 saw the highest for 457 TV Shows.

Our analysis on movies duration showed that movies ranging between 90mins to 150mins were the highest with 3481 movies followed by movie duration less than 90mins with 1653 movies and finally movies with more than 150mins duration has 243 movies.

Coming to the main part processing the text data using NLTK library and performing those actions on description feature. After that we have removed all the stop words and applied stemming to it (Stemming is the process of reducing a word to its word stem that affixes to suffixes and prefixes or to the roots of words known as a lemma). After that finding lengths of features and storing new features for clustering.

Standardized all the data before performing Ml Model in this case we used Kmeans algorithm because after seeing the analysis done we thought this is the algorithm can balance all the features. Plotted Silhouette for the optimal Kvalues and Elbow plot for cluster size and we found out the optimal clusters can be used are 21.

Performed Recommender systems using cosine similarity because The cosine similarity is beneficial because even if the two similar data objects are far apart by the Euclidean distance because of the size, they could still have a smaller angle between them. Smaller the angle, higher the similarity.

The recommendations after all the tuning and model selection we are getting pretty good range of recommendations and satisfied with the recommendations.

The given Netflix dataset has been successfully analysed and visualised by various plots and charts and the final result recommendations are very positive.
