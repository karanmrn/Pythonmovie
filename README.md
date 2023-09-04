# Pythonmovie
Movie Recommendation System Documentation

Overview
This notebook provides tools for movie search and recommendations. It first allows users to search for movies based on titles, and then recommends movies based on the behavior of users who liked the searched movie.

Table of Contents
Data Loading and Initial Exploration
Data Cleaning
Vectorizing Titles
Building a Search Function
Interactive Widget for Movie Search
Recommending Movies Based on User Behavior
Interactive Widget for Movie Recommendations

1. Data Loading and Initial Exploration <a name="data-loading-and-initial-exploration"></a>
Modules Used: pandas
Dataset: movies.csv
Description: Loads a dataset of movies into a DataFrame for further processing and displays the first five rows.

3. Data Cleaning <a name="data-cleaning"></a>
Modules Used: re
Function: clean_title(title)
Description: Cleans a movie title by removing non-alphanumeric characters. This cleaned title is stored in a new column in the DataFrame.

4. Vectorizing Titles <a name="vectorizing-titles"></a>
Modules Used: sklearn.feature_extraction.text.TfidfVectorizer
Description: Converts the cleaned movie titles into a matrix of TF-IDF features for similarity computations.

5. Building a Search Function <a name="building-a-search-function"></a>
Modules Used: sklearn.metrics.pairwise.cosine_similarity, numpy
Function: search(title)
Description: Accepts a movie title as input and returns the top 5 movies from the dataset that are most similar to the given title. The similarity is determined using cosine similarity.

7. Interactive Widget for Movie Search <a name="interactive-widget-for-movie-search"></a>
Modules Used: ipywidgets, IPython.display
Widgets: movie_input, movie_list
Description: Provides an interactive text box for users to type movie titles. As the user types, the system displays similar movie titles below the input box.

9. Recommending Movies Based on User Behavior <a name="recommending-movies-based-on-user-behavior"></a>
Function: find_similar_movies(movie_id)
Description: Recommends movies based on the behavior of users who liked the given movie. The system identifies users who liked the input movie and then finds other movies these users liked. It returns a list of recommended movies.

11. Interactive Widget for Movie Recommendations <a name="interactive-widget-for-movie-recommendations"></a>
Modules Used: ipywidgets, IPython.display
Widgets: movie_name_input, recommendation_list
Description: Provides an interactive text box for users to search for movies. When a movie title is entered, the system displays recommended movies based on similar user behavior.

This documentation provides a comprehensive guide to the movie recommendation system presented in the notebook.
