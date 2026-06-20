# Polynomial Regression — Position Level vs Salary

A machine learning project demonstrating Polynomial Regression
to predict employee salaries based on their position level.

## 📌 Problem Statement
Predict salary based on employee position level.
Linear regression fails here because salary growth is 
non-linear — it accelerates sharply at senior levels.

## 📊 Dataset
- Source: Position Salaries Dataset
- Rows: 10
- Features: Position, Level, Salary
- Target: Salary

| Column   | Description              |
|----------|--------------------------|
| Position | Job title                |
| Level    | Numeric level (1 to 10)  |
| Salary   | Annual salary            |

## 🔍 Approach
1. EDA — visualized Level vs Salary curve
2. Fit Linear Regression as baseline
3. Applied Polynomial Features (degree 1 to 6)
4. Added Ridge regularization to control overfitting
5. Compared R² across all degrees

## 📈 Results

| Degree | R²     |
|--------|--------|
| 1      | 0.61   |
| 2      | 0.86   |
| 3      | 0.93   |
| 4      | 0.97   |
| 6      | 0.9962 |

### Final Model (Degree 6 + Ridge)
| Metric | Value     |
|--------|-----------|
| R²     | 0.9962    |
| MAE    | ₹8,196    |
| RMSE   | ₹11,843   |

## 🔑 Key Learnings
- Linear regression (R² 0.61) badly underfit the salary curve
- Polynomial features captured the non-linear growth pattern
- Ridge regularization kept coefficients controlled at higher degrees
- R² improved consistently from degree 1 → 6 confirming the 
  non-linear relationship

## 🛠️ Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## 📁 Project Structure
