# Movie Recommendation System

This project is a content-based movie recommendation system built in Python. It leverages the TF-IDF (Term Frequency-Inverse Document Frequency) vectorization technique and cosine similarity to suggest movies similar to the user's favorite movie. Given a movie title, the system finds and returns movies with similar genres, keywords, taglines, cast, and director.

## Project Overview

The goal of this recommendation system is to provide movie suggestions based on the content of the movies. This approach does not rely on user interaction data but instead uses descriptive features such as genres, keywords, tagline, cast, and director to find similarities between movies.

## Features

- **TF-IDF Vectorization**: Converts the combined text data into feature vectors using the `TfidfVectorizer`.
- **Cosine Similarity Calculation**: Computes similarity scores between movies based on their TF-IDF vectors.
- **Flexible Matching**: Uses `difflib` to match the closest title to user input, handling misspellings or partial titles.
- **Content-Based Recommendations**: Leverages TF-IDF and cosine similarity to compare movies by their descriptive features, offering highly relevant suggestions.
- **Top Recommendations**: Displays the top 30 similar movies, helping users discover new titles based on the chosen movie's attributes.

## Requirements

- Python 3.x
- numpy
- pandas
- scikit-learn

  ## Work Flow
  ![image](https://github.com/user-attachments/assets/fb207fe0-9c45-47f1-adb8-9ce26825c4e4)

## How It Works

## 1.Data Loading and Exploration 
  Loads movie data from the CSV file into a DataFrame for exploration and analysis.
  
## 2.Feature Selection and Preprocessing:
  Chooses key content attributes: genres, keywords, tagline, cast, and director.
  Fills missing values with an empty string to handle any missing data gracefully.
  Combines selected features into a single text feature, preparing them for vectorization.
  
## 3.Text Vectorization:
  TF-IDF Vectorizer: Converts combined text features into numerical vectors, highlighting important words while reducing noise from common terms.
  
## 4.Similarity Calculation:
  Cosine Similarity: Measures the similarity between movie vectors. A high cosine similarity score means the movies share similar attributes, while a low score indicates 
  fewer common features.
  
## 5.Title Matching & Recommendation:
  Matches user input to the closest movie title using difflib, handling slight variations in title spelling.
  Retrieves and ranks movies by similarity, outputting the top 30 recommendations.

## 📝 Example Usage

Enter your favourite movie name: Inception

Movies suggested for you:

1. Inception
2. Interstellar
3. The Dark Knight
4. The Matrix
5. Shutter Island
