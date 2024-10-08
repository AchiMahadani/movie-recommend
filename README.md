# Movie Recommendation System

This repository implements a **Movie Recommendation System** that provides personalized movie suggestions to users based on their preferences. The system leverages collaborative filtering techniques and content-based filtering to enhance user experience by recommending movies tailored to their tastes.

## Project Overview

In the era of streaming platforms, an effective recommendation system is crucial for enhancing user engagement. This project aims to deliver personalized movie recommendations by analyzing user preferences, ratings, and movie features. By combining collaborative filtering with content-based filtering, the system can make recommendations based on user interactions and the inherent characteristics of the movies themselves.

### Key Features:
- **Collaborative Filtering**: Recommends movies based on user-user or item-item similarity, leveraging user ratings and interactions.
- **Content-Based Filtering**: Suggests movies by analyzing movie features such as genre, director, and cast, aligning them with user preferences.
- **Hybrid Approach**: Combines collaborative and content-based filtering for improved recommendations.
- **Top-N Recommendations**: Provides a list of the top N recommended movies for each user.
- **Scalable Architecture**: Designed to handle large datasets with efficient recommendation algorithms.

## Recommendation Approaches

This system combines both **Collaborative Filtering** and **Content-Based Filtering** to provide accurate and diverse recommendations:

- **Collaborative Filtering**: This approach is based on the assumption that users who have agreed on movies in the past will also agree on movies in the future. The system predicts a user's preference for a movie by identifying similar users (user-based) or finding similar movies (item-based).
  
- **Content-Based Filtering**: Each movie is described by its attributes, such as genre, actors, director, etc. The system recommends movies with similar features to those the user has already liked or watched.

### Collaborative Filtering
We implement both **User-User** and **Item-Item** collaborative filtering:
- **User-User Filtering**: Finds users with similar movie preferences and recommends movies they have enjoyed.
- **Item-Item Filtering**: Identifies movies that are similar to the ones a user has liked in the past.

### Content-Based Filtering
Movies are recommended based on the metadata (e.g., genre, actors) of the movies a user has previously rated highly. 

## Dataset

The dataset used in this project is the (https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata), a widely-used dataset for building recommendation systems. It includes user ratings for thousands of movies.


### Preprocessing:
- **Handling Missing Data**: Filling missing values in movie metadata.
- **Normalization**: Scaling user ratings to ensure consistency in the model.
