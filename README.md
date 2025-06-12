# Titanic
This repository contains my solution to the [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic/overview) competition on Kaggle. The goal of the project is to predict the survival of passengers aboard the Titanic based on various features.

## Project Structure

- **`train.csv`**: Training dataset provided by Kaggle.
- **`test.csv`**: Test dataset provided by Kaggle.
- **`titanic_solution.ipynb`**: Jupyter Notebook containing data preprocessing, feature engineering, model training, and evaluation.
- **`best_params.json`**: JSON file containing the best hyperparameters for the models used in the Stacking Classifier.
- **`submission.csv`**: Final submission file with predictions for the test dataset.

## Methodology

1. **Data Preprocessing**:
   - Handling missing values.
   - Encoding categorical variables.
   - Feature scaling and engineering.

2. **Model Training**:
   - Multiple machine learning models were trained and evaluated, including:
     - Logistic Regression (L1 and L2 regularization)
     - Random Forest
     - XGBoost
   - A **Stacking Classifier** was used to combine the predictions of these models for improved performance.

3. **Hyperparameter Tuning**:
   - Hyperparameters were optimized using grid search and K-fold cross-validation.
   - The optimal parameters are stored in `best_params.json`.

4. **Submission**:
   - Predictions were made using the trained Stacking Classifier and saved in `submission.csv`.
