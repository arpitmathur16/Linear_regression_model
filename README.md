# Linear Regression Model

A beginner-friendly, well-documented walkthrough of **Linear Regression** using scikit-learn — built on the classic Diabetes dataset to predict disease progression from patient body metrics.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/arpitmathur16/Linear_regression_model/blob/main/Linear_Regression.ipynb)

##  Overview

This notebook explains Linear Regression from the ground up — not just the code, but the *why* behind each step. Every section includes a "What Did We Observe?" and "What Did We Learn?" breakdown, making it a good reference for anyone learning ML fundamentals.

**Problem Statement:** Predict a patient's disease progression score based on their body metrics (BMI, Blood Pressure, Blood Sugar Level), so doctors can identify patients who may need early intervention.

##  Dataset

The project uses scikit-learn's built-in **Diabetes dataset** (`sklearn.datasets.load_diabetes`), reduced to four columns:

| Column | Description |
|---|---|
| `BMI` | Body Mass Index |
| `Blood_Pressure` | Average blood pressure |
| `Blood_Sugar_Level` | Blood sugar measurement (s6) |
| `Disease_Progression` | Target variable — quantitative measure of disease progression |

##  Tech Stack

- **NumPy** — numerical operations
- **Pandas** — data handling (DataFrames)
- **Matplotlib & Seaborn** — data visualization
- **Scikit-learn** — model building and evaluation

##  Workflow

1. **Import Libraries** — load NumPy, Pandas, Matplotlib, Seaborn, and Scikit-learn
2. **Load & Inspect Data** — load the diabetes dataset and preview its shape and structure
3. **Exploratory Data Analysis (EDA)**
   - Histogram of BMI distribution
   - Scatter plot: BMI vs. Disease Progression
   - Correlation heatmap across all features
4. **Data Cleaning** — inject and impute a missing value (mean imputation), check for duplicates
5. **Feature Selection** — define `X` (BMI, Blood Pressure, Blood Sugar Level) and `y` (Disease Progression)
6. **Train-Test Split** — 80/20 split with `random_state=42` to avoid data leakage
7. **Model Building & Training** — fit a `LinearRegression()` model on the training set
8. **Predictions** — generate predictions on the test set and compare against actual values
9. **Evaluation Metrics**
   - Mean Absolute Error (MAE)
   - Root Mean Squared Error (RMSE)
   - R² Score
10. **Performance Visualization**
    - Actual vs. Predicted scatter plot
    - Residual plot
11. **Conclusion & Beginner ML Dictionary** — summary of results plus a glossary of key ML terms (feature, target, training/testing data, etc.)

##  Results

- **R² Score:** > 0.99
- **Mean Absolute Error:** well under 1.0 points

These results indicate a very strong linear relationship between the selected features and disease progression in this dataset.

##  How to Run

**Option 1: Google Colab (recommended)**
Click the "Open In Colab" badge above to run the notebook directly in your browser.

**Option 2: Local setup**
```bash
git clone https://github.com/arpitmathur16/Linear_regression_model.git
cd Linear_regression_model
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
jupyter notebook Linear_Regression.ipynb
```

##  Key Concepts Covered

- Supervised learning fundamentals
- Exploratory Data Analysis (EDA)
- Handling missing data
- Train-test split & data leakage
- Ordinary Least Squares (OLS) fitting
- Regression evaluation metrics (MAE, RMSE, R²)
- Residual analysis

##  Author

**Arpit Mathur**
- GitHub: [@arpitmathur16](https://github.com/arpitmathur16)
- LinkedIn: [arpit-mathur16](https://linkedin.com/in/arpit-mathur16)

##  License

This project is open for educational use. Feel free to fork and build on it.
