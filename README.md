# Anime-Recommended-System

This project builds a personalized anime recommendation system using both content-based and collaborative filtering techniques. With the growing number of anime titles and diverse viewer preferences, the goal is to improve user satisfaction and engagement through accurate recommendations.

📊 Overview
We developed a hybrid recommendation system that integrates:

Content-Based Filtering using a Random Forest Regressor

Collaborative Filtering using KNNWithMeans and Singular Value Decomposition (SVD)

Clustering for user segmentation with K-Means

Hybrid Model combining content-based and collaborative predictions

🧠 Machine Learning Techniques
Content-Based Filtering
Model: Random Forest Regressor

Inputs: Genre, Type, Episodes, Average Rating, Popularity

Initial MSE: 1.96

After genre consolidation: MSE increased to 2.11 due to underfitting

Unsupervised Clustering
Technique: K-Means (k=62)

Features: Genre, Popularity

Revealed meaningful genre/popularity-based groupings

Suggested use of PCA for better scalability

Collaborative Filtering
Methods:

KNNWithMeans (best with k=50, Pearson similarity) → RMSE: 1.43

SVD → RMSE: 1.39

Hybrid Model
Blend: 30% Random Forest + 70% SVD

Achieved best RMSE: 1.32

Demonstrated benefits of integrating even a weaker content-based model

🗂️ Dataset
The dataset includes:

Anime metadata (genres, type, episodes, average community rating, popularity)

User rating data

📈 Results
Best performing model: Hybrid (RF + SVD)

Final RMSE: 1.32

🔧 Future Improvements
Apply dimensionality reduction (e.g., PCA) for clustering

Explore deep learning-based recommendation systems

Refine genre and metadata encoding
