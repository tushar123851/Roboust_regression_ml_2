# 🏠 House Price Prediction Using Machine Learning Regression Models

## 📌 Project Overview

This project focuses on building a complete machine learning pipeline to predict house prices using multiple regression algorithms. The project includes data preprocessing, feature engineering, model training, model evaluation, visualization, and model comparison.

Different machine learning models were implemented and compared to identify the most effective model for house price prediction.

---

<div align="center">
  
![Python](https://img.shields.io/badge/Python-3.10-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

</div>

---

# 📖 Project Overview

This project builds a complete machine learning pipeline to predict house prices using various regression algorithms.

The workflow includes:

✅ Data preprocessing  
✅ Outlier handling  
✅ Feature scaling  
✅ Model training  
✅ Model evaluation  
✅ Cross-validation  
✅ Visualization  
✅ Model comparison  

The main objective is to compare multiple regression algorithms and select the most effective model for house price prediction.

[![Watch Demo](https://img.shields.io/badge/🎥%20Watch%20Project%20Demo-Click%20Here-red?style=for-the-badge)](https://drive.google.com/drive/folders/1VbHiUBmptPLns8Nc0NsEFouMxqECvlVh?usp=drive_link)


---

# 🎯 Project Objectives

- Predict house prices accurately
- Handle missing values and outliers
- Apply feature scaling
- Compare multiple regression algorithms
- Reduce overfitting
- Evaluate model performance
- Select the best prediction model

---

# 📂 Dataset Information

Dataset features:

| Feature |
|-----------|
| Area (sqft) |
| Bedrooms |
| Bathrooms |
| Location Score |
| Property Age |
| Distance from City |
| Near School |
| Near Metro |
| Crime Rate Index |
| House Price |

### Target Variable

```text
house_price_inr
```

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Programming Language |
| Pandas | Data Processing |
| NumPy | Numerical Operations |
| Matplotlib | Visualization |
| Scikit-Learn | Machine Learning |
| Jupyter Notebook | Development |

---

# ⚙ Data Preprocessing Workflow

### Step 1: Import Dataset

```python
df = pd.read_csv("house_price.csv")
```

### Step 2: Handle Missing Values

```python
df.isnull().sum()
```

Performed:

- Numerical value handling
- Categorical value handling

### Step 3: Remove Unnecessary Columns

```python
df.drop(
['property_id','sale_date'],
axis=1,
inplace=True
)
```

### Step 4: Remove Outliers

Method Used:

```python
IQR Method
```

### Step 5: Feature Scaling

```python
scaler=StandardScaler()

df[scaling_column]=scaler.fit_transform(
df[scaling_column]
)
```

---

# 🤖 Machine Learning Models Implemented

## 1️⃣ Decision Tree Regression

Decision Tree Regression creates tree-based decision rules and predicts target values.

### Advantages

- Easy interpretation
- Handles non-linear relationships
- No scaling required

---

## 2️⃣ Random Forest Regression

Random Forest combines multiple decision trees to improve performance.

### Advantages

- High accuracy
- Low overfitting
- Strong generalization

---

## 3️⃣ Ridge Regression (L2)

Ridge applies L2 regularization.

### Advantages

- Reduces overfitting
- Controls coefficient size
- Improves stability

---

## 4️⃣ Lasso Regression (L1)

Lasso applies L1 regularization.

### Advantages

- Feature selection
- Reduces complexity
- Controls overfitting

---

## 5️⃣ Support Vector Regression (SVR)

SVR predicts values using support vectors and margins.

### Advantages

- Works well on complex data
- Effective with scaling
- Strong generalization

---

# 📊 Evaluation Metrics Used

## R² Score

Measures prediction accuracy.

Formula:

R² = 1 − SSR/SST

---

## Mean Absolute Error (MAE)

Measures average prediction error.

Formula:

MAE = Σ|Actual − Predicted| / n

---

## Mean Squared Error (MSE)

Measures squared prediction error.

Formula:

MSE = Σ(Actual − Predicted)² / n

---

## Cross Validation Score

Measures model stability across multiple folds.

---

# 📈 Model Performance Comparison

| Model | Train R² | Test R² | CV Score | MAE | MSE |
|---------|----------|----------|----------|----------|----------------|
| Decision Tree | 93.53% | 90.39% | 90.13% | 1,919,489.71 | 6,276,877,760,903 |
| Random Forest | 94.72% | 92.05% | 92.11% | 1,723,283.63 | 5,191,255,598,488 |
| Ridge Regression | 91.45% | 91.02% | 91.29% | 1,876,064.31 | 5,861,972,049,605 |
| Lasso Regression | 91.45% | 91.02% | 91.29% | 1,876,064.29 | 5,861,971,810,920 |
| Support Vector Regression | 91.35% | 91.13% | 90.28% | 1,855,717.45 | 5,792,911,744,612 |

---

# 🏆 Final Results

### Best Model Selected

# Random Forest Regression

Performance:

| Metric | Value |
|----------|---------|
| Training Score | 94.72% |
| Testing Score | 92.05% |
| Cross Validation | 92.11% |

Reasons:

✅ Highest prediction accuracy

✅ Lowest prediction error

✅ Very low overfitting

✅ Strong generalization capability

---

## 👤 Author

**Tushar Vala**  
📊 Data Science Enthusiast  
🐍 Python | Pandas | Machine Learning  

---

)
