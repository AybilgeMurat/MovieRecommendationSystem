# MovieRecommendationSystem
It was developed with MOVILENS' 100K dataset and Surprise library. A content-based and collaborative-based recommendation system was used.

Data Set
Among the data sets published by MOVILENS; The data set with 100k votes (1-5), 943 users and a total of 1682 films was used in this project. The data set contains data such as age, gender, occupation in the user file. Each user has rated at least 20 movies. In the movie data set, there are attributes such as id, movie name and types of movies for each movie. there is no metadata to summarize the movie for the movies in the 100k dataset. 
Therefore, only movie types will be used for content-based filtering.

![image](https://user-images.githubusercontent.com/58533563/187210268-d87cd2d1-e77d-4374-ac8c-abbe973b1c7e.png)

Attributes such as profession, gender, release date of the film that will not be used in the project will not be included in the data frames that will be newly created by going through the ver selection stage, as mentioned in the information discovery process.

![image](https://user-images.githubusercontent.com/58533563/187210379-69631b7b-95f5-4b4d-a5e3-48719c348ccc.png)


There are 19 unique film types in the data set. The genre distribution of films was shown on a graph. Here, the list we created for the species was used.


![image](https://user-images.githubusercontent.com/58533563/187210563-a638b9d7-eab2-444f-b086-57a4c8e7b297.png)


In the project, the weighted rating formula used by IMDB in the popularity-based recommendation system was used.


![image](https://user-images.githubusercontent.com/58533563/187210707-a5c3060f-b1dc-4796-ba1c-e0acf666773a.png)


We see that the most popular movie is Star Wars. Indeed, when we look at it, it is obvious that the 10 films on the list are also films that have been watched a lot and have received good votes.

![image](https://user-images.githubusercontent.com/58533563/187210747-2ca0427e-e6fd-4b45-b52a-231a9e7c0323.png)

Another method used in the project is content-based filtering. Since there are no words to summarize the films in the data set here, the operations were performed over genres. When definitions are made, the recommendation process is performed by calculating similarities in the film-type matrix using the cosine similarity method mentioned.


![image](https://user-images.githubusercontent.com/58533563/187211008-0235c67a-e7f5-4091-a08f-070e3b9b8bdf.png)


The Surprise library was used for collaborative filtering. The library offers us many popular approaches ready-made. The approaches such as SVD and KNN mentioned while making the definitions were used in the project. The results are visible at the end of the project.
