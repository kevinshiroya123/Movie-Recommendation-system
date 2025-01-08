# Movie-Recommendation-system
This project implements a Movie Recommendation System using a content-based approach enhanced with the FAISS library for scalable nearest neighbor search. The system uses the TMDB dataset and recommends movies based on genres, popularity, vote count, and storyline similarity.

Overview:

This project implements a content-based movie recommendation system that ranks movies based on:

Genres: Prioritized for stronger recommendations.
Popularity: Ensures relevance.
Storyline Similarity: Matches similar plots and keywords.
Vote Count: Considers movies with significant user engagement.
The system is built using Python, leverages FAISS for scalable similarity search, and processes over 900,000 movie records from the TMDB dataset.


Features
Dynamic Genre Matching: Combines genres of movies matching the query title for personalized recommendations.
Popularity Threshold: Focuses on highly popular movies (e.g., top 20% by popularity).
Efficient Search with FAISS: Handles large datasets efficiently, offering real-time recommendations.
Weighted Recommendation:
Higher weights for genres and popularity.
Balanced consideration for vote count and storyline.


Dataset Details
Source:
Dataset: TMDB Movies Dataset 2023
Size: ~930,000 movie records
Key Columns Used:
Title: Movie title.
Overview: Brief plot description.
Genres: Movie genres (e.g., Action, Comedy).
Keywords: Keywords associated with the movie.
Popularity: Popularity score.
Vote Count: Number of votes received.
Preprocessing:
Missing Data:
Filled missing overview, genres, and keywords with empty strings.
Dropped rows with missing title.
Normalization:
Scaled popularity and vote_count for better weighting.
Combined Features:
Combined genres, keywords, and overview for similarity calculations.


Performance and Runtime
Dataset Size: 930,000+ movies.
Preprocessing Time: ~2 minutes (depends on system).
Recommendation Runtime:
Real-time recommendations (milliseconds) using FAISS.



Here’s the entire README content in plain text for direct copy-pasting into your README.md file:

Movie Recommendation System
A scalable content-based movie recommendation system using FAISS for efficient similarity search and a preprocessed TMDB dataset. The system dynamically combines genres, popularity, and storyline to generate personalized movie recommendations.

Table of Contents
Overview
Features
Dataset Details
Project Architecture
Installation and Setup
Usage
Performance and Runtime
Examples
Contributing
License
Overview
This project implements a content-based movie recommendation system that ranks movies based on:

Genres: Prioritized for stronger recommendations.
Popularity: Ensures relevance.
Storyline Similarity: Matches similar plots and keywords.
Vote Count: Considers movies with significant user engagement.
The system is built using Python, leverages FAISS for scalable similarity search, and processes over 900,000 movie records from the TMDB dataset.

Features
Dynamic Genre Matching: Combines genres of movies matching the query title for personalized recommendations.
Popularity Threshold: Focuses on highly popular movies (e.g., top 20% by popularity).
Efficient Search with FAISS: Handles large datasets efficiently, offering real-time recommendations.
Weighted Recommendation:
Higher weights for genres and popularity.
Balanced consideration for vote count and storyline.
Dataset Details
Source:
Dataset: TMDB Movies Dataset 2023
Size: ~930,000 movie records
Key Columns Used:
Title: Movie title.
Overview: Brief plot description.
Genres: Movie genres (e.g., Action, Comedy).
Keywords: Keywords associated with the movie.
Popularity: Popularity score.
Vote Count: Number of votes received.
Preprocessing:
Missing Data:
Filled missing overview, genres, and keywords with empty strings.
Dropped rows with missing title.
Normalization:
Scaled popularity and vote_count for better weighting.
Combined Features:
Combined genres, keywords, and overview for similarity calculations.


Performance and Runtime
Dataset Size: 930,000+ movies.
Preprocessing Time: ~2 minutes (depends on system).
Recommendation Runtime:
Real-time recommendations (milliseconds) using FAISS.


Examples
Input:
Movie Title: Batman
Number of Recommendations: 10

Output:
Title	Genres	Popularity	Vote Count
Batman: Bad Blood	Action,Crime	12.121	818
Batman: Mask of the Phantasm	Animation,Action	20.015	967
Batman: Hush	Action,Crime	13.657	786
Batman: Mystery of the Batwoman	Animation,Action	27.447	345
Batman Beyond: The Movie	Animation,Action	7.887	171


License
This project is licensed under the MIT License.


