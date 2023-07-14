## Song Genre Classification

## Introduction
With the rise of streaming services, music lovers are often overwhelmed by the extensive music libraries available to them. To tackle this challenge, streaming platforms rely on techniques like audio analysis to categorize songs and offer personalized recommendations. In this project, we will explore The Echo Nest dataset, aiming to classify songs as 'Hip-Hop' or 'Rock' without listening to them, solely based on the provided data(using audio characteristics).

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

## Methodology
The methodology for developing an end-to-end classification model to predict the genre of a song based on its audio features involved the following steps:

1. Data Loading and Exploratory Data Analysis (EDA):
   - Loaded the dataset containing audio features of songs.
   - Performed basic data exploration to understand the structure of the data.
   - Visualized the distributions and relationships between variables to gain insights into the data.

2. Preprocessing:
   - Removed unnecessary columns that are not relevant for genre classification.
   - Handled class imbalances if present in the dataset to ensure balanced representation of genres.
   - Normalized the data to bring all features to a similar scale for better model performance.

3. Dimensionality Reduction with PCA:
   - Applied Principal Component Analysis (PCA) to reduce the dimensionality of the feature space.
   - Select the principal components that capture a cumulative variance of 85%.
   - This step helps in reducing computational complexity and removing noise from the data.

4. Model Selection:
   - Choosed appropriate machine learning algorithms for classification, such as Decision Trees, Logistic Regression, and Support Vector Machines (SVM).
   - Evaluated the suitability of each algorithm based on their performance characteristics, interpretability, and the nature of the dataset.

5. Model Evaluation:
   - Evaluated the performance of each model using classification metrics such as precision, recall, and F1-score.
   - Applied cross-validation techniques to assess the model's generalization capability and reduce overfitting.
   - Splited the dataset into training and testing sets to evaluate how well the model generalizes to unseen data.

6. Hyperparameter Tuning:
   - Fine-tuned the selected models by optimizing their hyperparameters.
   - Used techniques like grid search to explore different combinations of hyperparameters.
   - Find the best combination that maximizes the model's performance metrics on the validation set.

7. Saving the Best Performing Model:
   - Selected the best performing model(Support Vector Machines) based on the evaluation metrics.
   - Saved the trained model to be used for future predictions or deployments.

## Results:
The developed end-to-end classification model(SVM) achieved an accuracy of 85.05%,indicating that it correctly predicted the genre for 85% of the songs in the dataset. and an area under the curve (AUC) of 0.9209 suggests that the model has a strong ability to distinguish between different song genres based on their audio features.Both genres have an F1-score of 0.86, indicating a balanced performance between precision and recall for both genres.Overall, based on these evaluation metrics, the model demonstrates good performance in correctly predicting the genres of Hip-Hop and Rock songs.
