## Song Genre Classification

## Context
This project focuses on classifying songs into different genres using machine learning techniques. The dataset consists of audio features of songs, such as acousticness, danceability, energy, instrumentalness, liveness, speechiness, tempo, valence, and the corresponding genre labels.

## Dataset
The dataset used for this project contains 4802 rows and 10 columns. The columns include:

* acousticness: a measure of the acoustic quality of the song

* danceability: a measure of how suitable the song is for dancing based on a combination of musical elements

* energy: a measure of the intensity and activity of the song

* instrumentalness: a measure of whether the song is instrumental or contains vocals

* liveness: a measure of the presence of a live audience in the recording

* speechiness: a measure of the presence of spoken words in the song

* tempo: the tempo of the song in beats per minute (BPM)

* track_id: unique identifier for each song

* valence: a measure of the musical positivity of the song

* genre_top: the genre label assigned to each song

## Project Overview
The project aims to develop an end-to-end classification model to predict the genre of a song based on its audio features. The project includes the following steps:

* Data Loading and Exploratory Data Analysis (EDA): Load the dataset, perform basic data exploration, and visualize the distributions and relationships between variables.

* Preprocessing: Removed unnecessary columns, handled class imbalances and normalized the data.

* PCA : Performed Principal component analysis for dimension reduction and selected the variables that captured a cumulative variance of 85%.

* Model Selection: Select appropriate machine learning algorithms for classification, such as Decision Trees, Logistic Regression, and Support Vector Machines (SVM).

* Model Evaluation: Evaluate the performance of each model using classification metrics, such as precision, recall, and F1-score. Apply cross-validation to ensure the model's generalization capability.

* Hyperparameter Tuning: Fine-tune the models by optimizing hyperparameters to improve their performance. Use techniques like grid search or random search to find the best combination of hyperparameters.

* Saving the best performing model(SVM).
