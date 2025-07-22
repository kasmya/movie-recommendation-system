# Movie Recommendation System

A content-based movie recommendation system built using the TMDB 5000 dataset. It suggests movies similar to a given title by analyzing features like genres, cast, keywords, director, and overview.

## Overview

This project uses metadata to recommend similar movies without relying on user ratings. It processes key descriptive features from the dataset, combines them into a single text field, and uses cosine similarity to rank movie similarity.

## How It Works

- Merged and cleaned the TMDB movies and credits datasets
- Extracted important features: `genres`, `keywords`, `cast`, `director`, and `overview`
- Combined all features into a single `tags` field for each movie
- Vectorized the text using `CountVectorizer`
- Calculated cosine similarity scores between movies
- Built a simple recommendation function based on similarity ranking

## Technologies Used

- Python  
- Pandas, NumPy  
- Scikit-learn  
- CountVectorizer  
- Cosine Similarity  
- Jupyter Notebook

## Dataset

- [TMDB 5000 Movie Dataset (Kaggle)](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

## Future Improvements
 
- Explore hybrid recommendation methods  
- Add evaluation metrics like precision@k or recall@k  

## How to Run

1. Clone the repository  
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

