# 🚗 Car Model Prediction Using Machine Learning

This project builds a machine learning classification model that predicts a car’s model/category based on various features from a real dataset. The goal is to apply proper preprocessing, encode categorical data, train multiple ML algorithms, and compare their performance using standard evaluation metrics.

---

## 📊 Dataset

The dataset (`UserCarData.csv`) includes features such as:

- Region  
- State / Province  
- City  
- Fuel type  
- Seller type  
- Transmission  
- Torque  
- Sold status  
- Car model (used as target label)

---

## 🛠 Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Scikit-Learn**

---

## 🧹 Data Preprocessing

Steps performed:

1. Load the dataset with Pandas  
2. Drop unnecessary columns  
3. Apply **one-hot encoding** using `pd.get_dummies()`  
4. Split the dataset into train/test sets  

---

## 🤖 Models Used

Three ML models were trained and compared:

### 🔹 Decision Tree Classifier  
- Tuned with `max_depth=10`  
- Evaluated using accuracy & confusion matrix  

### 🔹 Logistic Regression  
- Used to test linear model performance  

### 🔹 Gaussian Naive Bayes  
- Performs well with high-dimensional encoded data  

---

## 📈 Evaluation

Each model is evaluated using:

- Accuracy Score  
- Classification Report  
- Confusion Matrix  

This helps determine which classifier performs best on the dataset.

---

## 📂 Project Structure

