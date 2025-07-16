# 🚢 Titanic Survival Prediction - Kaggle Project

This project is a machine learning pipeline to predict survival outcomes on the Titanic dataset provided by Kaggle. The goal is to apply data preprocessing, feature engineering, and classification algorithms to predict which passengers survived the disaster.

---

## 📂 Project Overview

This repository contains a Jupyter Notebook that walks through the full data science process:

1. 📥 Load and explore the dataset  
2. 🧹 Clean and preprocess data  
3. 🛠️ Engineer useful features  
4. 🤖 Train a logistic regression model  
5. 📊 Evaluate performance  
6. 📤 Generate predictions for Kaggle submission

---

## 📑 Dataset

The dataset comes from the [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic/) competition on Kaggle.

Files used:
- `train.csv` - training set with labels
- `test.csv` - test set (for submission)

---

## ⚙️ Methods Used

### 📊 Data Preprocessing

- Filled missing values (`Age`, `Embarked`)
- Removed non-informative columns: `Cabin`, `Ticket`, `Name`
- Converted categorical columns (`Sex`, `Embarked`) to numeric using `get_dummies`
- Created new features like:
  - `FamilySize` = `SibSp` + `Parch` + 1
  - `IsAlone` = (`FamilySize` == 1)

### 🤖 Model Training

- **Logistic Regression** via `scikit-learn`
- Data split: 80% training, 20% validation (`train_test_split`)
- Model evaluated using **accuracy score**

### 🧪 Evaluation

- Used accuracy metric to measure performance
- Cross-validation or advanced metrics (e.g., confusion matrix, ROC) can be added as extensions

---

## 🚀 Getting Started

### 🔧 Requirements

- Python 3.x
- Jupyter Notebook
- `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`

External dataset URL:(https://www.kaggle.com/datasets/heptapod/titanic)
