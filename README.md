# 🏠 House Price Prediction & Car Model Classification (Machine Learning Project)

This project includes two major machine learning tasks:

1. **Car Model Classification** – predicting the car’s model based on multiple features  
2. **House Price Prediction** – predicting the selling price using regression models  

Both tasks include preprocessing, feature encoding, training ML models, and evaluating performance.

---

# 📌 1. Car Model Classification

## 📊 Dataset
The dataset (`UserCarData.csv`) includes:

- Region  
- State / Province  
- City  
- Fuel type  
- Seller type  
- Transmission  
- Torque  
- Whether the car was sold  
- Car name (Target for classification)

## 🧹 Data Preprocessing
- Dropped irrelevant columns (e.g., `owner`)
- Applied **one-hot encoding** with `pd.get_dummies()`
- Train-test split (80/20)

## 🤖 Classification Models Used
You trained and evaluated:

- Decision Tree Classifier  
- Logistic Regression  
- Random Forest Classifier  
- KNN Classifier  
- Gaussian Naive Bayes  
- Support Vector Classifier (RBF, Linear, Polynomial kernels)

## 📈 Evaluation
Metrics include:

- Accuracy score  
- Confusion matrix (visualized using Seaborn heatmap)  
- Classification report  
- Precision (weighted, macro)

---

# 📌 2. House Price Prediction (Regression)

## 🎯 Objective
Predict the **selling price** of a house/property using numerical and categorical features.

## 🧹 Data Preprocessing
- One-hot encoding of:
  - Region  
  - State  
  - City  
  - Fuel type  
  - Seller type  
  - Transmission  
  - Torque  
  - Sold  
  - Car name (included for regression)
- Dropped the target column to form X and y:
  - **X = features**
  - **y = selling_price**

- Train-test split

## 🤖 Regression Models Used

### 🔹 Lasso Regression  
Regularized linear regression (L1).

### 🔹 Ridge Regression  
Regularized linear regression (L2).

### 🔹 Linear Regression  
Baseline regression model.

### 🔹 Gradient Boosting Regressor  
Tree-based boosting model for improved accuracy.

## 📈 Evaluation
For each regression model, the notebook outputs:

- Training score  
- Test score  
- Predictions on test data  

---

# ⚙️ Hyperparameter Tuning
Used **GridSearchCV** on Decision Tree:

- Parameters tuned:
  - `max_depth`
  - `min_samples_split`
- Performed 5-fold cross-validation

---

# 📂 Project Structure

