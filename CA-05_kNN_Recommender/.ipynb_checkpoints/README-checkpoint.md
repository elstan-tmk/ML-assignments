# CA05 - KNN based Movie Recommender Engine

## 1. The Application

At Scale, this would look like recommending products on Amazon, articles on Medium, movies on Netflix, or videos on Youtube. <br>
Although, they all use more efficient means of making recommendations due to the enormous volume of data they process. <br>
However, we would replicate one of these recommender systems on a smaller scale using what we have learned. <br>

## 2. Data Source and Contents
Since we are not working at they big companies, we could not grab the data from the data warehouse, we have to get our data through some other means. <br>

We are going to use:<br>

<u>Data File Name: </u> movies_recommendation_data.csv <br>
<u>File Location: </u> https://github.com/ArinB/MSBA-CA-Data/raw/main/CA05/movies_recommendation_data.csv <br>

The data contains thirty movies, including data for each movie across seven genres and their IMDB ratings. <br>
The labels column values are all zeroes because we are not using this data set for classification or regression. <br>
The implementation assumes that all columns contain numerical data. <br>
<br>
Additionally, there are relationships among the movies that will not accounted for (e.g. actors, directors, and themes),
when using the KNN algorithm simply because the data that captures those relationships are missing from the data set.<br>
Consequently, when running the kNN algorithm on the data, similarity will be based solely on the included genres and the IMDB ratings of the movies.

## 3. Building the own Recommender System

The movie recommendation webite will be built by using the Recommendation Engine at the back-end.<br>
Imagine a user is navigating the recommendation website, and this user encounters a movie named "The Post".<br>
The user is not sure if he/she wants to watch it, but its genres intrigue the user;<br>
The user is curious about other similar movies. The user scrolls down to the "More Like This" section to see what recommendations your recommendation website will make, and the back-end algorithmic gears begin to turn.<br><br>

Your website sends a request to its back-end for the 5 movies that are most similar to "The Post".<br>
The back-end has a recommendation data set exactly like ours.<br>
It begins by creating the row representation (better known as a <b>feature vector</b> for <i>The Post</i>,<br>
then it runs a program similar to the one to search for the 5 movies that are most similar the <i>The Post</i>,<br>
and finally sends the results back to the user at the website.

![image](https://user-images.githubusercontent.com/75411111/228690370-4abbe5f6-a6d4-447f-a6a4-14437cfac481.png)

