# **Wine Quality Prediction**

This repository contains the code and resources for predicting wine quality based on physicochemical properties using machine learning algorithms. The project explores various classification techniques, evaluates their performance, and optimizes models for better accuracy.

---

## **Table of Contents**
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Models and Methods](#models-and-methods)
- [Results](#results)
- [Setup and Usage](#setup-and-usage)
- [Future Work](#future-work)
- [License](#license)

---

## **Project Overview**
The goal of this project is to predict the quality of red and white wines on a scale of 3 to 9 based on their physicochemical attributes. Machine learning techniques such as Logistic Regression, Random Forest, and XGBoost are applied to achieve high accuracy and interpretability.

---

## **Dataset**
The dataset used for this project is the [Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/wine+quality) from the UCI Machine Learning Repository. It consists of:
- **Features**: 12 physicochemical properties (e.g., pH, alcohol, residual sugar).
- **Target**: Quality ratings (3–9).
- **Samples**: 1,599 red wines and 4,898 white wines.

### **Preprocessing Steps**
1. Removed duplicates.
2. Addressed class imbalance using SMOTE.
3. Standardized numerical features.

---

## **Models and Methods**
The following machine learning algorithms were applied:
1. **Logistic Regression**: A baseline model for comparison.
2. **Random Forest**: An ensemble method for robust classification.
3. **XGBoost**: A high-performance gradient boosting algorithm.

### **Optimization**
- Hyperparameter tuning was performed for Random Forest and XGBoost using RandomizedSearchCV.

---

## **Results**
| **Model**            | **Accuracy** | **F1-Score** | **Remarks**                  |
|-----------------------|--------------|--------------|------------------------------|
| Logistic Regression   | 82%          | 0.79         | Baseline performance.        |
| Random Forest         | 88%          | 0.85         | Significant improvement.     |
| XGBoost               | 91%          | 0.89         | Best performance achieved.   |

- **Feature Importance**: Alcohol content and volatile acidity were the most predictive features.

---

## **Setup and Usage**

### **Prerequisites**
- Python 3.x
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `xgboost`, `imblearn`, `matplotlib`, `seaborn`, `joblib`.

### **Steps**
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/wine-quality-prediction.git
   cd wine-quality-prediction
