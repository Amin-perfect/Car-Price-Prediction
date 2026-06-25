# Used Car Price Prediction

## The Problem
Pricing a used car isn't straightforward. Two cars of the same model can be worth very different amounts depending on age, mileage, fuel type, transmission, and how many previous owners it's had. Buyers and sellers often rely on rough intuition this project replaces that guesswork with a model trained on real patterns in the data.

## The Goal
Predict a used car's fair resale price from its specifications, using a dataset of real listings with features like:
- Manufacturing year
- Present (original) price
- Kilometers driven
- Fuel type
- Seller type
- Transmission type
- Number of previous owners

## The Challenge: Mixed Data Types
Unlike purely numeric datasets, this one mixes numeric features (year, mileage) with categorical ones (fuel type, transmission, seller type). Categorical features can't be fed directly into a regression model, so a key part of this project was **encoding** these categories into a numeric form the model could actually learn from — without losing the meaning behind them.

## Approach
1. **Data Cleaning** — handled inconsistent entries and verified feature ranges made sense (e.g., no negative mileage)
2. **Feature Encoding** — converted categorical columns (fuel type, seller type, transmission) into numeric representations
3. **Correlation Analysis** — used a heatmap to identify which features most strongly influenced selling price
4. **Train-Test Split** — held out test data to evaluate real-world generalization
5. **Model Training** — trained a Linear Regression model on the encoded feature set
6. **Evaluation** — assessed performance using R² score

## Result
The model achieved an **R² score of 0.78** on the test set meaning it explains 78% of the variation in car selling prices using the available features alone.

## What I'd Improve Next
Trying a Random Forest or Gradient Boosting regressor to capture non-linear pricing patterns (e.g., depreciation that isn't perfectly linear with age), and comparing the result against this baseline Linear Regression model.

## Tech Stack
Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Jupyter Notebook

## Author
Amin (Mr. PerfecT) BSCS Student | Aspiring Data Scientist & AI Developer
