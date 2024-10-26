# project_movie_recommendation_system

This recommendation system recommends different movies to users. Since this system is based on a collaborative approach, it will give progressively explicit outcomes contrasted with different systems that are based on the content-based approach. Content-based recommendation systems are constrained to people, these systems don't prescribe things out of the box. These systems work on individual users’ ratings, hence limiting your choice to explore more. While our system which is based on a collaborative approach computes the connection between different clients and relying upon their ratings, prescribes movies to others who have similar tastes, subsequently allowing users to explore more.
First, a new user is provided with a screen that contains a search bar that allows him to search for a particular movie.

![image](https://github.com/varun98b/project_movie_recommendation_system/assets/51908568/635ed161-cdf8-4f3b-9a9f-1d21ab07f8b6)
Web UI streamlit application

In the next step, we find the index value of the movie selected by the user from the pivot table we created and give it to the model to find the K Nearest Neighbors to find the similar ratings given by other users to other movies. In particular, we are considering the K value as 6. 
Using the object in which the KNN model is created, the indices and the distances of the K Nearest Neighbors are calculated. As the K value is 6 we should the top 6 values and give the respected movie names as recommendations to the user for the movie he/she selected in the web UI.

