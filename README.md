# Movie Recommendation System
This project implements a content-based movie recommendation system using machine learning techniques.

## Dataset
The project uses two datasets from TMDB (The Movie Database):
* tmdb_5000_credits.csv
* tmdb_5000_movies.csv

  These datasets contain information about 5000 movies, including details like budget, genre, keywords, cast, crew, and user ratings.

## Approach
### Content-Based Filtering: 
  content-based filtering by computing the movie overviews using TF-IDF vectorization.
  Finally, compute the cosine similarity between the TF-IDF vectors of movie overviews to find movies that are content-wise similar.
  This creates personalized recommendations based on movie features like plot, cast, crew, director, and genres.

## Procedure
  1.Data preprocessing and merging of the two datasets
  
  2.Handling missing values
  
  3.Feature engineering to extract relevant information from complex fields (e.g., cast, crew, genres)
  
  4.Implementation of demographic filtering using weighted ratings
  
  5.Creation of a TF-IDF matrix for movie overviews
  
  6.Calculation of cosine similarity between movies
  
  7.Implementation of content-based filtering using movie metadata

## Models and Techniques Used
* TF-IDF (Term Frequency-Inverse Document Frequency) Vectorization: For creating TF-IDF matrix from movie overviews
* Cosine Similarity: For calculating similarity between movies 
* CountVectorizer: For creating a count matrix from movie metadata
## Results
The system can provide movie recommendations based on:
* Overall popularity and ratings
* Content similarity to a given movie

Example recommendations:

  For "The Dark Knight Rises": Other Batman movies, superhero films
  
  For "The Avengers": Other Marvel movies, superhero ensemble films
  
  For "Minions": Other animated family comedies

## Future Improvements
* Incorporate user preferences for personalized recommendations
* Add a collaborative filtering approach
* Create a user interface for easier interaction
  
    This project demonstrates the basics of content-based recommendation systems and can be extended for more sophisticated applications.
