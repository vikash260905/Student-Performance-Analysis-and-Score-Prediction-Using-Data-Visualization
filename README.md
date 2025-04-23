# 🎓 Student Performance Analysis and Score Prediction Using Data Visualization

This project analyzes student performance data using **exploratory data analysis (EDA)** and visualizations, then builds a **Linear Regression model** to predict math scores. It helps in identifying performance trends, high and low performers, and subject-wise score distributions.

---

## 🧹 Data Cleaning Steps

1. **Load the Dataset:**
   - CSV file: `student-scores python.csv`

2. **Check Data Structure:**
   - Used `df.info()` and `df.describe()` for basic understanding.

3. **Handle Missing and Duplicate Data:**
   - `df.dropna(inplace=True)` — Removed rows with missing values.
   - `df.drop_duplicates(inplace=True)` — Removed duplicate records.

4. **Identify Numeric Columns:**
   - Used `df.select_dtypes(include='number')` to extract columns with scores.

---

## 📊 Visualizations

### ✅ Exploratory Data Analysis (EDA)

| Visualization Type | Purpose |
|--------------------|---------|
| **Histogram**      | Distribution of scores for each subject |
| **Box Plot**       | Identify outliers and spread of scores |
| **Bar Chart**      | Average score comparison across subjects |
| **Pie Chart**      | Subject-wise contribution to overall performance |
| **Scatter Plot**   | Relationship between two subject scores |
| **Line Graph**     | Scores of the first 10 students across subjects |
| **Heatmap**        | Correlation between different subject scores |

### 🏅 Performance Highlights

- **Top 5 Performing Students**: Based on `total_score` column.
- **Bottom 5 Performing Students**: Based on `total_score` column.
- **Ranked Subjects**: Based on average scores using horizontal bar chart.

---

## 🤖 Machine Learning Model

### 📌 Goal: Predict `math_score` using other subject scores

- **Model Used**: `LinearRegression` from `sklearn`
- **Train-Test Split**: 80/20 using `train_test_split`
- **Evaluation Metrics**:
  - **Mean Squared Error (MSE)**
  - **R² Score**

### 📈 Actual vs Predicted Plot
Visual representation of model performance comparing actual scores with predicted values.

---

## 🧰 Libraries Used

```python
pandas
matplotlib
seaborn
scikit-learn

📍 Conclusion & Results
Students' performance varies significantly between subjects.

Strong correlations observed between some subjects, which can be useful for predicting missing or future scores.

The Linear Regression model showed reasonable accuracy in predicting math scores using other subject scores.

Visualizations helped in identifying trends, top performers, and weak subjects across the dataset.

🚀 How to Use
