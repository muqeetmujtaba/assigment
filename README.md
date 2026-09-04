# ❤️ Framingham Heart Disease Classification

## 📌 Project Overview

This project focuses on developing a **Machine Learning Classification System** to predict whether a patient is at risk of developing **Coronary Heart Disease (CHD) within the next 10 years**.

The project uses the **Framingham Heart Study dataset** and follows a complete machine learning workflow, including:

* Data Analysis
* Data Preprocessing
* Missing Value Handling
* Encoding
* Feature Scaling
* Class Imbalance Handling
* Multiple Classification Models
* Model Performance Comparison
* Hyperparameter Tuning
* Final Model Selection
* Classification Report
* Confusion Matrix

---

## 🎯 Objective

The main objective of this project is to build and evaluate classification models that can predict the target variable:

**`TenYearCHD`**

Where:

* `0` → Patient is not predicted to develop CHD within 10 years
* `1` → Patient is predicted to develop CHD within 10 years

The project also aims to improve model performance through preprocessing, balancing techniques, and hyperparameter optimization.

---

## 📊 Dataset

The project uses the **Framingham Heart Study dataset**.

### Dataset Information

* **Total Records:** 4,238
* **Total Features:** 16
* **Target Variable:** `TenYearCHD`

### Features

The dataset contains patient-related health and lifestyle information such as:

* Age
* Gender
* Education
* Current Smoker
* Cigarettes Per Day
* Blood Pressure Medication
* Previous Stroke
* Hypertension
* Diabetes
* Total Cholesterol
* Systolic Blood Pressure
* Diastolic Blood Pressure
* Body Mass Index
* Heart Rate
* Glucose Level

---

## 🔄 Machine Learning Workflow

### 1. Data Loading

The dataset is loaded using Pandas and initially analyzed to understand its structure and contents.

### 2. Exploratory Data Analysis

The dataset is analyzed using:

* `head()`
* `shape`
* `info()`
* `describe()`
* Missing value analysis
* Duplicate detection
* Target distribution analysis

### 3. Missing Value Handling

Missing values are identified and handled using **median imputation** for numerical features.

This helps preserve the dataset without unnecessarily removing valuable records.

### 4. Duplicate Removal

Duplicate records are identified and removed to improve data quality.

### 5. Encoding

Categorical features are converted into numerical form using **One-Hot Encoding** where required.

### 6. Train-Test Split

The dataset is divided into:

* **80% Training Data**
* **20% Testing Data**

Stratified splitting is used to preserve the target class distribution.

### 7. Feature Scaling

`StandardScaler` is applied to standardize numerical features.

Scaling is particularly useful for models such as:

* Logistic Regression
* SVM
* KNN

### 8. Handling Class Imbalance

The target variable is imbalanced because the number of patients without CHD is significantly higher than patients with CHD.

To address this issue, **SMOTE (Synthetic Minority Over-sampling Technique)** is applied to the training data.

SMOTE creates synthetic samples for the minority class and produces a more balanced training dataset.

> SMOTE is applied only to the training data to avoid data leakage.

---

## 🤖 Classification Models

Multiple classification algorithms are implemented and compared:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Extra Trees Classifier
5. Gradient Boosting
6. Support Vector Machine (SVM)
7. K-Nearest Neighbors (KNN)

---

## 📈 Model Evaluation

Each model is evaluated using the following metrics:

### Accuracy

Measures the percentage of total predictions that are correct.

### Precision

Measures how many of the patients predicted as positive actually belong to the positive class.

### Recall

Measures how many actual positive cases were correctly identified.

### F1-Score

Provides a balance between Precision and Recall.

### Classification Report

A complete classification report is generated containing:

* Precision
* Recall
* F1-Score
* Support

### Confusion Matrix

A confusion matrix is generated to visualize:

* True Positives
* True Negatives
* False Positives
* False Negatives

---

## 🏆 Model Selection

The models are compared based on their performance across multiple evaluation metrics.

For this medical classification problem, **Recall and F1-Score are given particular importance**, because correctly identifying patients who may be at risk of CHD is important.

The best-performing model is selected based on the overall evaluation results.

---

## ⚙️ Hyperparameter Tuning

After comparing the initial models, hyperparameter tuning is performed on the selected model.

Techniques such as:

* `GridSearchCV`
* Cross-validation
* Parameter optimization

can be used to find the best combination of model parameters.

The goal is to improve the model's:

* Accuracy
* Precision
* Recall
* F1-Score

while reducing overfitting.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Imbalanced-learn
* Jupyter Notebook

---

## 📁 Project Structure

```text
Framingham-Heart-Disease-Classification/
│
├── framingham.csv
├── Framingham_Heart_Disease_Classification.ipynb
├── README.md
└── requirements.txt
```

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/framingham-heart-disease-classification.git
```

Navigate to the project directory:

```bash
cd framingham-heart-disease-classification
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn imbalanced-learn jupyter
```

---

## ▶️ How to Run

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Framingham_Heart_Disease_Classification.ipynb
```

Then run the notebook cells sequentially.

---

## 📊 Evaluation Metrics

The project generates:

* Accuracy Score
* Precision Score
* Recall Score
* F1-Score
* Classification Report
* Confusion Matrix
* Model Comparison Visualization

---

## 🔍 Key Learning Outcomes

Through this project, the following machine learning concepts are demonstrated:

* Data preprocessing
* Missing value imputation
* Categorical encoding
* Feature scaling
* Train-test splitting
* Imbalanced classification
* SMOTE
* Classification algorithms
* Model evaluation
* Confusion matrix analysis
* Cross-validation
* Hyperparameter tuning
* Model optimization
* Model comparison

---

## ⚠️ Disclaimer

This project is developed for **educational and machine learning purposes only**.

The predictions generated by this model should **not be considered medical advice or a clinical diagnosis**. Real-world medical applications require proper clinical validation and regulatory approval.

---

## 👨‍💻 Author

**Abdul Muqeet**

### ⭐ If you find this project useful, consider giving the repository a star!
