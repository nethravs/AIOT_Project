## HARPY INTERN AIOT PROJECT 1

***Recommendation System Model 1: Graph Neural Network (GNN) Based Model***


This recommendation system leverages a Graph Neural Network (GNN) architecture to predict movie preferences. It integrates user and movie embeddings 
with GNN layers for enhanced recommendation accuracy.

 **Dataset:**

MovieLens 100k from TensorFlow Datasets (TFDS) with user ratings (movie_title, user_id, timestamp) and movie titles.


**Features:**
The MovieLens 100k dataset from TensorFlow Datasets (TFDS) contains user ratings for movies, including features like movie_title, user_id, and timestamp 
for ratings, and movie_title for movies.

**Features:**

 - User and Movie Embeddings: Embeddings for users and movies are learned using TensorFlow's Embedding layers.

 * Graph Neural Network Layer: A custom GNNLayer aggregates embeddings based on user-movie interactions.

 + Retrieval Task: The retrieval task is evaluated using top-K metrics to measure recommendation accuracy.

 - Brute-Force Search for Retrieval: A brute-force search layer retrieves the top recommendations for a given user.

 * Visualization: Pie charts visualize the top 3 movie recommendations for specific users.Training metrics (loss, top-K accuracy) are plotted to assess
model performance over epochs.

 
***Recommendation System Model 2: K-Nearest Neighbour(KNN) Based Model***

This recommendation system uses a K-Nearest Neighbors (KNN) approach to predict movie preferences, leveraging user and movie embeddings 
for improved recommendations.

**Dataset:**

MovieLens 100k from TensorFlow Datasets (TFDS) with user ratings (movie_title, user_id, timestamp) and movie titles.

**Features:**

- User and Movie Embeddings: Embeddings for users and movies are learned using TensorFlow's Embedding layers.

* KNN Layer: Custom KNNLayer identifies and averages embeddings of the k-nearest neighbors.

+ Retrieval Task: The retrieval task uses top-K metrics to evaluate recommendation accuracy.

- Brute-Force Search for Retrieval: A brute-force search layer retrieves top recommendations for a given user.

* Visualization: Frequency polygons visualize the top recommendations for specific users.Training metrics (loss) are plotted to assess model
performance over epochs.

 


***Recommendation System Model 3: Session Based Recommendation Model***

This model recommends movies based on session data using user and movie embeddings to improve recommendation accuracy.

**Dataset:**

The MovieLens 100k dataset from TensorFlow Datasets (TFDS) contains user ratings for movies, including features like movie_title, user_id, and timestamp 
for ratings, and movie_title for movies.

**Features:**

- User and Movie Embeddings: Embeddings are created for users and movies using TensorFlow's Embedding layers to represent their latent features.

* Session-Based Modeling: The model incorporates session data, considering recent user interactions to enhance recommendation relevance.

+ Custom Task Layer: Uses a retrieval task with FactorizedTopK metrics to evaluate the model's recommendation accuracy.

- Brute-Force Search for Retrieval: A brute-force search mechanism retrieves top movie recommendations for users based on their session data.

* Column Graph Visualization: Visualizes the top movie recommendations for specific users using column graphs to show the frequency
of recommended titles.













    
