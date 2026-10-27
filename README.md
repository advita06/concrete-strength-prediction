# Concrete Compressive Strength Prediction

## Project Overview

This project uses Machine Learning to predict the compressive strength of concrete based on its material composition and age using a **Random Forest Regression** model.

The project uses the Concrete Compressive Strength dataset from Kaggle, which contains 1,030 records and 9 columns, including 8 input features and 1 target variable.

## Problem Statement

To develop a regression model that estimates the compressive strength of concrete using its ingredients and age, helping understand how different material properties influence concrete strength.

## Dataset

- **Source:** Kaggle — Concrete Compressive Strength Dataset
- **Total Records:** 1,030
- **Total Columns:** 9
- **Input Features:** 8
- **Target Variable:** Concrete compressive strength (MPa)

The dataset includes features related to cement, blast furnace slag, fly ash, water, superplasticizer, coarse aggregate, fine aggregate, and age.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Preprocessing

The following preprocessing steps were performed:

1. Loaded and explored the dataset using Pandas.
2. Checked for missing values and duplicate records.
3. Cleaned column names by removing unnecessary spaces.
4. Separated the input features (`X`) from the target variable (`y`).
5. Split the dataset into 80% training data and 20% testing data.

## Machine Learning Model

**Algorithm:** Random Forest Regressor

Model configuration:

- `n_estimators = 100`
- `random_state = 42`

The Random Forest model combines predictions from multiple decision trees to estimate concrete compressive strength.

## Model Evaluation

The model was evaluated using four regression metrics on the test dataset.

| Metric | Result |
|---|---:|
| Mean Absolute Error (MAE) | 3.4979 MPa |
| Mean Squared Error (MSE) | 27.6173 MPa² |
| Root Mean Squared Error (RMSE) | 5.2552 MPa |
| R² Score | 0.9074 |

## Key Findings

- The model achieved an **R² score of 0.9074**, explaining approximately 90.74% of the variation in concrete compressive strength in the test dataset.
- The **MAE of 3.4979 MPa** indicates that the average absolute prediction error was approximately 3.50 MPa.
- The **RMSE of 5.2552 MPa** measures prediction error while penalizing larger errors more heavily.
- The results demonstrate that Random Forest Regression can model relationships between concrete composition, age, and compressive strength effectively on this dataset.

## Conclusion

The Random Forest Regression model achieved strong predictive performance on the test dataset. With an R² score of 0.9074 and an MAE of approximately 3.50 MPa, the model provides a useful estimate of concrete compressive strength based on the available input features.

This project demonstrates a complete introductory regression workflow, including data exploration, preprocessing, model training, and performance evaluation.

## Limitations and Future Improvements

- Compare Random Forest with Linear Regression, Decision Tree, and Gradient Boosting models.
- Use cross-validation to evaluate model stability.
- Perform hyperparameter tuning to explore potential performance improvements.
- Analyze feature importance to understand which concrete ingredients contribute most to predictions.

## How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn jupyter
   ```

3. Open the Jupyter Notebook in VS Code or Jupyter Notebook.
4. Ensure the dataset is available at the file path specified in the notebook.
5. Run the notebook cells in order.

## Dataset Source

[Kaggle — Concrete Compressive Strength Dataset](https://www.kaggle.com/datasets/elikplim/concrete-compressive-strength-data-set)

## Disclaimer

This project is intended for educational purposes. Predictions should not replace standardized laboratory testing or engineering validation when assessing concrete for structural applications.

