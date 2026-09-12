# Titanic-survival-prediction

Goal: Predict whether a passenger survived the Titanic disaster using demographic and travel data (class, age, sex, fare, family relations, etc.) — a classic binary classification problem and one of the most well-known entry points into applied machine learning.

Dataset: Kaggle's Titanic dataset — passenger records including age, sex, ticket class, fare, cabin, and family relationships aboard.

Approach:

Feature engineering: Extracted Title from passenger names (Mr, Mrs, Miss, Master, etc.) as a proxy for social status and age group; engineered family_size from sibling/spouse and parent/child counts; bucketed Age_category to capture non-linear age effects on survival.
Modeling: Trained and compared Random Forest, Gradient Boosting, and XGBoost classifiers.
Tuning: Used GridSearchCV to optimize hyperparameters across all three models.

Result: Leaderboard score of 0.78229.

What this project demonstrates: Feature engineering from raw/unstructured fields (names → titles), handling mixed categorical and numerical data, and systematic model comparison with cross-validated hyperparameter tuning.
