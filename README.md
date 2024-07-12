# Movie Recommendation System

## Overview
This project implements a content-based movie recommendation system using Python. The system leverages movie metadata such as genres, keywords, cast, and crew to suggest similar movies based on content similarity. It preprocesses data to extract meaningful features, applies text processing techniques like stemming, and computes cosine similarity between movies to generate recommendations.

## Features
- **Data Preprocessing:** Cleans and preprocesses movie metadata, handling missing values and converting JSON strings.
- **Text Processing:** Utilizes NLTK's PorterStemmer for stemming to normalize tags and reduce word variations.
- **Feature Extraction:** Uses CountVectorizer to convert textual data into a matrix of token counts, focusing on important features while removing common English stop words.
- **Similarity Calculation:** Computes cosine similarity between movies based on their feature vectors to determine movie similarities.
- **Recommendation Functionality:** Provides a function to recommend movies similar to a given movie title, based on computed similarities.

## Usage
1. **Setup:** Ensure Python environment with necessary libraries (`numpy`, `pandas`, `scikit-learn`, `nltk`) is installed.
2. **Data Loading:** Load movie metadata from CSV files (`movies.csv`, `credits.csv`).
3. **Processing:** Preprocess data, extract relevant features, and compute cosine similarity.
4. **Recommendation:** Use the `recommend` function to suggest similar movies based on a provided movie title.

## Future Improvements
- Implement TF-IDF for better term weighting.
- Optimize similarity computation for large datasets using approximate nearest neighbors.
- Enhance user interface for interactive recommendations.
