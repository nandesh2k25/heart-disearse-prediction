# ❤️ Heart Disease Prediction using Machine Learning

## 📌 Project Overview

This project focuses on predicting the presence of heart disease using machine learning models.  
It includes:

- Data exploration and visualization
- Feature preprocessing
- Model training and evaluation
- Performance comparison between models

The dataset used is the Heart Disease dataset derived from the Cleveland dataset available at the UCI Machine Learning Repository.

---

## 📂 Dataset

- File: `data/heart.csv`
- Target variable: `Heart Disease`
    - 0 → No Heart Disease
    - 1 → Heart Disease

The dataset contains medical attributes such as:

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Max Heart Rate
- Exercise Induced Angina
- ST Depression
- Number of Major Vessels
- Thalassemia Test Results
- and others

---

## 🔍 Project Workflow

### 1️⃣ Data Exploration

- Display dataset information
- Statistical summary (`describe()`)
- Missing value check
- Unique value inspection
- Renaming columns for better readability
- Mapping categorical values to meaningful labels

---

### 2️⃣ Data Visualization

The following visualizations are performed:

- Histograms for distribution analysis
- Boxplots for outlier detection
- IQR-based outlier identification
- Count plots for class distribution
- Correlation heatmap
- Pairplot for feature relationships
- Scatter plots for feature interactions
- Pie chart for sex distribution

These visualizations help understand:
- Feature relationships
- Class separability
- Potential predictive variables
- Data imbalance

---

### 3️⃣ Data Preprocessing

- Feature-target separation
- Train-test split (80% training, 20% testing)
- Stratified splitting to preserve class distribution
- Feature scaling using StandardScaler

---

## 🤖 Machine Learning Models Used

### 1️⃣ Logistic Regression

A linear classification model used as a baseline.

### 2️⃣ Random Forest Classifier

Configured with:

- `n_estimators = 300`
- `max_depth = 6`
- `class_weight = 'balanced'`
- `random_state = 42`

This ensemble model reduces overfitting and improves prediction stability.

---

## 📊 Model Evaluation

Evaluation metrics:

- Training Accuracy
- Testing Accuracy
- Confusion Matrix

The confusion matrix visualizes:
- True Positives
- True Negatives
- False Positives
- False Negatives

Models are compared and sorted based on test accuracy.

---

## 📈 Key Learning Outcomes

- Understanding exploratory data analysis (EDA)
- Detecting and interpreting correlations
- Handling categorical feature mapping
- Preventing data leakage
- Using stratified sampling
- Comparing linear vs ensemble models
- Interpreting confusion matrices

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## ▶ How to Run

1. Clone the repository
2. Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn