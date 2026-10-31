# Student Pass/Fail Prediction Using Logistic Regression

## 📌 Project Overview

This project uses **Logistic Regression**, a Machine Learning classification algorithm, to predict whether a student belongs to the **Pass/Higher Performance** or **Fail/Lower Performance** category based on different student performance factors.

The project uses the **Student Performance Factors** dataset from Kaggle.

---

## 🎯 Objective

The main objective of this project is to build a Machine Learning classification model that predicts student performance.

The original dataset contains an `Exam_Score` column. Since Logistic Regression is used for classification, a new binary target variable called `Pass_Fail` is created.

- `1` → Pass / Higher Performance
- `0` → Fail / Lower Performance

The classification is created using the **median Exam Score as the threshold**.

---

## 📊 Dataset Features

The dataset contains student-related factors such as:

- Hours Studied
- Attendance
- Parental Involvement
- Access to Resources
- Sleep Hours
- Previous Scores
- Motivation Level
- Internet Access
- Tutoring Sessions
- Teacher Quality
- School Type
- Physical Activity
- Gender
- Exam Score

The `Exam_Score` column is used to create the `Pass_Fail` target and is not used as an input feature to avoid data leakage.

---

## ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🔄 Project Workflow

1. Load the dataset
2. Explore the dataset
3. Check missing values
4. Create the `Pass_Fail` target variable
5. Select input features and target
6. Handle missing values
7. Encode categorical features
8. Scale numerical features
9. Split the dataset into training and testing data
10. Train the Logistic Regression model
11. Make predictions
12. Evaluate the model using accuracy and classification metrics
13. Visualize results using a confusion matrix
14. Predict the result for a new student

---

## 🧹 Data Preprocessing

The dataset contains both numerical and categorical features.

### Numerical Features

Missing numerical values are handled using **median imputation**, followed by **Standard Scaling**.

### Categorical Features

Missing categorical values are handled using **most frequent value imputation**, followed by **One-Hot Encoding**.

A Scikit-learn **Pipeline** and **ColumnTransformer** are used to perform preprocessing and model training efficiently.

---

## 🤖 Machine Learning Model

The model used in this project is:

**Logistic Regression**

Logistic Regression is suitable for this project because the target variable has two classes:

- `0` → Fail / Lower Performance
- `1` → Pass / Higher Performance

---

## 📈 Model Evaluation

The model is evaluated using:

- Accuracy Score
- Classification Report
- Confusion Matrix

These metrics help measure how well the model predicts student performance.

---

## 📁 Project Structure

```text
Student_Pass_Fail_Prediction/
│
├── StudentPerformanceFactors.csv
├── logistic_regression_model.ipynb
├── README.md
```

---

## 📦 Installation

Install the required libraries:

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run the Project

1. Download or clone this repository.
2. Make sure `StudentPerformanceFactors.csv` is in the project folder.
3. Install the required libraries.
4. Open `logistic_regression_model.ipynb`.
5. Run all cells in order.

---

## 📌 Conclusion

This project demonstrates the complete Machine Learning workflow for a binary classification problem using Logistic Regression.

The model uses different student performance factors to classify students into two categories: **Pass/Higher Performance** and **Fail/Lower Performance**. The project also demonstrates important data preprocessing techniques such as handling missing values, encoding categorical data, scaling numerical features, and evaluating a Machine Learning model.

---

## 👩‍💻 Author

**Sejal K.**

AI & Data Science Engineering Student
