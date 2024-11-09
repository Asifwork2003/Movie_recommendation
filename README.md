# Movie Recommendation System

This project implements a simple movie recommendation system using K-Nearest Neighbors (KNN) based on movie ratings and features. It recommends movies to users by identifying similarities in ratings and item profiles.

## Features

- **Collaborative Filtering**: Recommends movies based on the ratings provided by similar users.
- **KNN Algorithm**: Uses KNN to find similar movies and generate recommendations.
- **TF-IDF Vectorization**: Helps in creating item profiles based on key features like genres, director, or common keywords from movie descriptions.

## How It Works

### Item Features

When building a recommendation system, it's important to understand the features of the items we're analyzing. These features could be common keywords from a text document or specific attributes of a movie such as its genre or director.

The goal is to match these features with those derived from users' actions and provide similar items with matching characteristics.

### Item Profile & TF-IDF

In order to compare features, we create an item profile, which is a summary of an item’s key features. To build this profile, we use **TF-IDF (Term Frequency - Inverse Document Frequency)**, which is a statistical measure used to evaluate the importance of a word in a document relative to a collection of documents.

- **TF (Term Frequency)**: Measures how often a word appears in a document relative to the total number of words.
- **IDF (Inverse Document Frequency)**: Rates how common or rare a word is across the corpus of documents. Rare words get higher scores, as they are more useful in differentiating items.

The formula for **TF-IDF** is: TF-IDF = TF × IDF

Where:
- **TF** = (Number of times term t appears in a document) / (Total number of terms in the document)
- **IDF** = log_e(Total number of documents / Number of documents with term t in it)

This score helps us identify which words or features best characterize an item, making it easier to compare and recommend similar items.

### Collaborative Filtering

Collaborative filtering is based on the idea that users who have agreed in the past will agree in the future. It recommends items to users based on preferences of users with similar tastes.

## Technologies Used

- **Python**  
- **Pandas**  
- **Scikit-learn**  
- **Scipy**  
- **Numpy**


