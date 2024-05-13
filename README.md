# Spotify-tracks-analysis

## Overview
This project focuses on evaluating the performance of different dimensionality reduction techniques and predicting if a person would like a particular song or not, using a classification model. The dataset includes features such as acousticness, danceability, energy, instrumentalness, liveness, speechiness, valence, and a binary label indicating whether a song is liked or not. The goal is to build the classification model and compare various dimensionality reduction techniques, and finally assess their accuracy, precision, recall, and F1-score.

## Data Analysis and Modeling
### Exploratory Data Analysis (EDA): 
The initial analysis involved exploring the distribution of features, correlations, and data preprocessing steps like handling missing values and encoding categorical variables.

### Modeling Approach:

#### Original Model: 
Used the complete feature set for training and testing the classification model.

#### Dimensionality Reduction Techniques:
1. Principal Component Analysis (PCA) with different numbers of components (PC-4, PC-3, PC-2)
2. Singular Value Decomposition (SVD) with different numbers of components (SVD-4, SVD-3, SVD-2)
3. Linear Discriminant Analysis (LDA)

## Model Evaluation:
1. Compared accuracy, precision, recall, and F1-score across different models and dimensionality reduction techniques.
2. Used Matplotlib library of Python to visualize and compare model performance metrics through bar plots.

## Results and Conclusions
### Accuracy Comparison:
1. The Original model had the highest accuracy, followed by PCA and SVD models.
2. LDA showed lower accuracy compared to other models.

### Precision and Recall:
1. Precision and recall varied across models, with PCA and SVD showing similar trends but lower than the Original model.
2. LDA had lower precision but slightly higher recall than PCA and SVD.

### F1-score:
The F1-score, a balanced measure of precision and recall, followed similar trends as precision and recall across models.

## Conclusion:
1. While dimensionality reduction techniques like PCA and SVD can reduce computational complexity, they may lead to a trade-off in model performance compared to the Original model.
2. LDA showed mixed performance, indicating challenges in achieving a balance between precision and recall.
