
# Song Genre Classification

## Project Overview
This project focuses on classifying songs based on features such as danceability, energy, acousticness, tempo, etc. into two music genres (Hip-Hop and Rock) using various machine learning techniques. The primary objective is to accurately predict the genre of a song based on its features. This repository contains the code, dataset, and documentation related to the project.

## Dataset
The analysis is based on two datasets:
- `echonest-metrics.json`: contains track metadata with genre labels
- `fma-rock-vs-hiphop.csv`: contains track metrics with the features

## Methods Used
- Dimensionality reduction using Principal Component Analysis (PCA).
- Machine Learning models:
  - Logistic Regression
  - Support Vector Machine (SVM)
  - Decision Tree (DT)
  - Random Forest (RF)

## Requirements
- Python 3.x
- Libraries:
  - pandas
  - NumPy
  - Matplotlib
  - seaborn
  - scikit-learn
  - joblib

## Installation and Usage
To set up the project, clone the repository and navigate to the directory. Run Jupyter Notebook to view the project:
```bash
git clone https://github.com/Shanmukhi1920/Song_Genre_Classification
cd Song_Genre_Classification
jupyter notebook
```
In Jupyter, open the `Song_Genre_Classification.ipynb` notebook.

## Notebook Overview
`Song_Genre_Classification.ipynb`: Contains the full analysis, from data loading, analysis and preprocessing to model building and evaluation.

## Results
**Performance Consistency:** Logistic Regression and SVM demonstrated consistent performance across cross-validation and test sets.

**Overfitting in Tree-based Models:** Decision Tree and Random Forest showed a significant difference in train and test accuracies, indicating potential overfitting.

**Hyperparameter Tuning:** Post-tuning, the Decision Tree and Random Forest models exhibited improved test set performance with accuracies around 82% and 85%, respectively.

**Insight on Model Tuning:** The Random Forest Classifier's test accuracy decreased slightly from 85.49% to 84.84% after tuning, highlighting that hyperparameter tuning does not always enhance performance. This serves as an important lesson in model optimization.
