# Movie-Recommendation-System

Dataset taken from "https://www.kaggle.com/datasets/utkarshx27/movies-dataset".

Purpose :
The aim of this project is to recommend the 30 most similar movies to a user-provided movie title based on various features such as genres, taglines, keywords, cast, and director. This system allows users to get relevant movie suggestions by simply entering the name of a movie they are interested in.

Technologies Used :
Python (for implementing the recommendation system)
scikit-learn (for machine learning models and vectorization)
pandas (for data manipulation and analysis)
difflib (for finding close matches between movie titles)
Google Colab (for development and testing)

Working :
Data Preprocessing: The project uses a dataset containing information about movies (sourced from Kaggle). Relevant features such as tagline, genres, keywords, cast, and director are extracted to determine the similarity between movies.

Feature Vectorization: We utilize TfidfVectorizer from scikit-learn to convert the text-based features into numerical values. This allows us to apply mathematical operations on them, which is essential for measuring similarity.

Similarity Calculation: Once the features are converted into numbers, Cosine Similarity is used to calculate the similarity score between the input movie and all other movies in the dataset. Cosine similarity is ideal for comparing text-based data, as it measures the angle between two vectors, determining how similar they are.

Movie Match & Sorting: The user inputs a movie name, and using difflib, we find the closest matches to the entered title from the dataset. After calculating the similarity score for each movie, the results are sorted, and the top 30 most similar movies are returned.

Dataset :
The dataset used in this project is a Movies Dataset taken from Kaggle. It contains information on thousands of movies, including details like title, genres, tagline, cast, director, and more. This data serves as the basis for calculating similarity scores and recommending the most relevant movies.

How It Works :
The user provides a movie title as input.
The system uses TfidfVectorizer to convert text data into numerical format.
Cosine Similarity is used to measure the closeness of other movies to the input.
difflib finds close matches for the movie title and sorts them based on similarity score.
The top 30 similar movies are displayed as recommendations.
