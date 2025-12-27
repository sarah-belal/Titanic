# Titanic Survival Prediction

This project applies machine learning techniques to predict passenger survival on the Titanic using the classic Kaggle Titanic dataset. The goal is to demonstrate an end-to-end supervised learning workflow, from data exploration to model training and evaluation.

## Problem Statement
Given passenger information such as ticket class, gender, and family relationships, the task is to predict whether a passenger survived the Titanic disaster.

This is a binary classification problem:
- `1` = Survived  
- `0` = Did not survive  

## Dataset
- Source: Kaggle Titanic Competition
- Files used:
  - `train.csv` — labeled training data
  - `test.csv` — unlabeled test data used for predictions

## Approach
1. Loaded and explored the dataset using pandas
2. Performed basic exploratory data analysis to identify important patterns
3. Selected key features:
   - Passenger class (`Pclass`)
   - Gender (`Sex`)
   - Number of siblings/spouses (`SibSp`)
   - Number of parents/children (`Parch`)
4. Encoded categorical variables using one-hot encoding
5. Trained a Random Forest classifier
6. Generated predictions for unseen test data
7. Created a submission file evaluated on Kaggle’s leaderboard

## Model
- Algorithm: Random Forest Classifier
- Library: scikit-learn
- Parameters:
  - Number of trees: 100
  - Maximum depth: 5

The model improves upon a simple gender-based baseline by incorporating multiple passenger features.

## Tools & Technologies
- Python
- pandas
- NumPy
- scikit-learn
- Kaggle Notebooks

## Results
The trained model successfully generates survival predictions for unseen passengers and achieves a competitive score on the Kaggle leaderboard, demonstrating a complete and reproducible machine learning pipeline.

## Files in This Repository
- `notebook.ipynb` — data exploration, model training, and prediction
- `submission.csv` — predictions submitted to Kaggle
- `README.md` — project overview and documentation

## Learnings
- Gained hands-on experience with supervised learning workflows
- Practiced feature selection and preprocessing
- Learned how to train and evaluate ML models using real-world data
- Used Kaggle as an experimentation and benchmarking platform
