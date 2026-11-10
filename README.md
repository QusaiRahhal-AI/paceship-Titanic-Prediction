# Spaceship Titanic Prediction

## Project Overview
An advanced machine learning classification pipeline built for the Kaggle competition to predict whether passengers were transported to an alternate dimension during a space collision event, leveraging complex feature engineering and missing data imputation.

## Dataset
- **Source:** Kaggle - Spaceship Titanic
- **Dataset Link:** [https://www.kaggle.com/competitions/spaceship-titanic]

## Pipeline Architecture & Methodology
1. **Data Integration & Cleaning:**
   - Merged training and test datasets temporarily to maintain consistent feature encoding dimensions.
   - Imputed missing values using domain-specific strategies (median for numerical attributes, mode/constant strings for categorical features).
2. **Advanced Feature Engineering:**
   - Extracted structural features from passenger cabins by splitting the `Cabin` string into Deck, Room Number, and Side.
   - Derived group sizes and family structures from `PassengerId`.
   - Aggregated spending across onboard services into a unified `Total_Spending` feature.
3. **Encoding & Modeling:**
   - Applied One-Hot Encoding to categorical variables.
   - Trained tree-based ensembles (Random Forest and XGBoost) optimized with robust hyperparameters.

## Results & Performance
- **Best Performing Model:** XGBoost
- **Key Metrics:** Achieved strong validation accuracy, demonstrating the effectiveness of advanced feature extraction in handling unstructured and sparse datasets.

## Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, XGBoost, Matplotlib, Seaborn# paceship-Titanic-Prediction
