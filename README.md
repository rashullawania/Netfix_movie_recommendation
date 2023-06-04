## Netflix_Movies_Recommendation

In this project, I have clustered similar movies and TV shows available on Netflix taking into account attributes like description, cast, director, genre etc. for a particular movie/show
## Project Files Description
This project includes a colab notebook, a data source and a presentation:
## Problem Statement
Netflix is the world’s leading internet entertainment service enjoying TV series, documentaries, and feature films across a wide variety of genres and languages. The task is to analyze the dataset from the Netflix database to cluster similar content by matching text-based features. Most users spend more time deciding what to watch than watching a movie or a TV show. Therefore, by understanding the existing data and analysing their trends and patterns, a machine learning model can be built for the segmentation of different types of movies/TV shows that can help the user in recommending movies and shows based on their preferences.
## Data Summary

This dataset consists of TV shows and movies available on Netflix as of 2019. The dataset is collected from Fixable which is a third-party Netflix search engine. In 2018, they released an interesting report which shows that the number of t shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset. Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

show_id : Unique ID for every Movie / TV Show

type : Identifier - A Movie or TV Show

title : Title of the Movie / TV Show

director : Director of the Movie

cast : Actors involved in the movie / show

country : Country where the movie / show was produced

date_added : Date it was added on Netflix

release_year : Actual Release Year of the movie / show

rating : TV Rating of the movie / show
duration : Total Duration - in minutes or number of seasons

listed_in : Genere

description: The Summary description
##  Approach:
Data cleaning and pre-processing: Here I checked and handled the missing and duplicate variables from the dataset as these can significantly affect the performance of a machine learning algorithm.

Exploratory Data Analysis: Here I wanted to learn the important statistical insights from the data where I checked for the distributions of the different attributes and their correlation with each other. I also performed univariate and bivariate analyses.

Clustering: Clustering or cluster analysis is a machine learning technique, which groups the unlabelled dataset. It can be defined as "A way of grouping the data points into different clusters, consisting of similar data points. The objects with the possible similarities remain in a group that has less or no similarities with another group." It does it by finding some similar patterns in the unlabelled dataset such as shape, size, colour, behaviour, etc., and divides them as per the presence and absence of those similar patterns. It is an unsupervised learning method, hence no supervision is provided to the algorithm, and it deals with the unlabeled dataset. After applying this clustering technique, each cluster or group is provided with a cluster-ID. ML systems can use this id to simplify the processing of large and complex datasets.
## Data Insights:
Most of the content available on Netflix is for mature audiences which shows the demand for kids’ content is low.
In recent years, Netflix has increasingly focused on TV shows rather than movies.
Most movies/TV shows available on Netflix were directed by Raúl Campos and Jan Suter.
Based on the content available on Netflix, the United States has produced the highest number of movies and TV shows.

Most movies’ duration is around 80 to 120 minutes whereas the duration for TV shows is around 1 to 2 seasons.Japan has more TV shows than movies on Netflix.
Anupam Kher has acted in most of the movies and shows present on Netflix.
Hierarchical clustering formed 4 clusters whereas K-means formed 5 clusters.
We get the optimal value of k at 5 using the elbow method and Silhouette score.
Content is divided into 5 clusters: Family movies, Documentaries, International TV Shows, International movies and Kids’ TV shows.
## Conclusion
In this project, we worked on a text clustering problem wherein we had to classify/group the Netflix shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

The dataset contained about 7787 records, and 11 attributes.

We began by dealing with the dataset's missing values and doing exploratory data analysis (EDA).

It was found that Netflix hosts more movies than TV shows on its platform, and the total number of shows added on Netflix is growing exponentially. Also, majority of the shows were produced in the United States

It was decided to cluster the data based on the attributes: director, cast, country, genre, and description. The values in these attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.

We first built clusters using the k-means clustering algorithm, and the optimal number of clusters came out to be 6. This was obtained through the elbow method and Silhouette score analysis.

A content based recommender system was built using the similarity matrix obtained after using cosine similarity. This recommender system will make 10 recommendations to the user based on the type of show they watched.
## Credits
RASHUL LAWANIA | Engineer | Machine Learning Enthusiast
