# Movie Rating Prediction

## Project Overview

This project builds an end-to-end machine learning pipeline
to predict whether a film will receive a high rating (≥ 7)
using metadata features.

The workflow includes:
- Data cleaning
- Feature engineering
- Model training
- Model evaluation
- Class imbalance handling

---

## Project Structure

movie-rating-prediction/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_engineering.ipynb
│   └── 02_modeling.ipynb
│
├── README.md
└── requirements.txt

---

## Data Engineering

- Fixed malformed CSV headers
- Handled missing numeric values
- Merged relational datasets
- Engineered cast size feature
- Created binary classification target

---

## Modeling

Models evaluated:
- Logistic Regression
- Logistic Regression (Scaled)
- Logistic Regression (Class Balanced)
- Decision Tree

### Final Model
Balanced Logistic Regression

Accuracy: ~73%  
Recall (High Rated Films): ~57%

---

## Key Insights

- Vote count and revenue strongly influence rating classification.
- Class balancing significantly improved detection of high-rated films.
- Logistic Regression outperformed Decision Tree in recall.

---

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- Ensemble models (Random Forest, Gradient Boosting)
