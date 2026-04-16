# Book-Recommendation-Using-KNN
This repository features a book recommendation system built using the Book-Crossing dataset and the K-Nearest Neighbours (KNN) algorithm from scikit-learn. The model recommends similar books based on user rating patterns, treating each book as a vector in a high-dimensional user space.

The dataset consists of over 1 million ratings across hundreds of thousands of books and users. To ensure statistical significance and reduce noise, the data is filtered according to the challenge requirements by retaining only users with at least 200 ratings and books with at least 100 ratings. The filtered ratings are then merged with book metadata and transformed into a user–book matrix using a pivot table.

The recommendation model is built using NearestNeighbors with cosine similarity as the distance metric and a brute-force search strategy. Cosine similarity is chosen due to the sparse and high-dimensional nature of the dataset, as it focuses on similarity in rating patterns rather than magnitude.

Key components include:
• Data Preprocessing: Filtering users and books based on rating frequency and constructing a clean user–book interaction matrix.
• Model Training: Applying KNN with cosine similarity on a sparse matrix representation of the dataset.
• Recommendation System: Retrieving the top 5 most similar books for a given title based on nearest neighbour distances.

This project is completed as part of the “Book Recommendation Engine using KNN” challenge from the Machine Learning with Python Certification by freeCodeCamp. The challenge is considered successful if the model produces a specific set of recommendations for a given test case.

Please note that this notebook is intended as a personal reference to the course materials provided. All credit for the course content and instructional materials goes to the course instructors.
