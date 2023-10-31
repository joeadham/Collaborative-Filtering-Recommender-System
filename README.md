## Movie Recommender System

This repository contains code to implement a collaborative filtering (CF) recommender system for recommending movies. The system is built using Python and utilizes user ratings from "ratings.csv" to generate movie recommendations from "movies.csv." Here's a brief overview of the project and its components.

### Introduction

In this project, we build a movie recommender system based on Collaborative Filtering. Collaborative Filtering is a technique that recommends items (in this case, movies) to users based on the preferences and behavior of other users. Specifically, we employ the cosine similarity function to calculate similarity between movies and make recommendations.

### Requirements

To use this project, you need the following files:
- `movies.csv`: Contains information about movies, including movie IDs and titles.
- `ratings.csv`: Contains user ratings for movies, including user IDs, movie IDs, and ratings.

### Getting Started

1. Clone the repository to your local machine:
   ```
   git clone https://github.com/yourusername/movie-recommender.git
   ```

2. Install the necessary libraries:
   ```
   pip install pandas numpy scikit-learn
   ```

3. Run the Jupyter Notebook `movie_recommender.ipynb` to see the code and results.

### Sections

1. **Importing Necessary Libraries:** Import required Python libraries, including pandas, numpy, matplotlib, and scikit-learn.

2. **Reading and Preprocessing the Dataset:** Load and preprocess the movie and rating data. We merge the two datasets, filter users and movies, and create a user-movie matrix.

3. **Calculating the Cosine Similarity Matrix:** Calculate the cosine similarity between movies to determine how similar they are to each other.

4. **Finding the Top 10 Similar Movies:** Demonstrate how to find the top 10 movies similar to a given movie, such as "Toy Story (1995)" or "Waiting to Exhale (1995)."

5. **Recommend Movies to a User:** Use the calculated similarity matrix to recommend 3 movies to a specific user (user ID 200 in this case).

### How It Works

- We start by creating a user-movie matrix with ratings, where rows represent users, columns represent movies, and cells contain user ratings.

- We calculate the cosine similarity between movies based on their ratings. This similarity matrix allows us to identify how similar two movies are in terms of user preferences.

- For a given movie, we find the top 10 most similar movies. This can be used to recommend movies that are similar to a movie of the user's choice.

- For a specific user (user ID 200 in this example), we recommend three movies based on their previously rated movies. We consider both the similarity of movies and the ratings the user has given.

---

Feel free to use, modify, and contribute to this movie recommender system project. If you have any questions or need assistance, please don't hesitate to reach out. Enjoy recommending movies!
