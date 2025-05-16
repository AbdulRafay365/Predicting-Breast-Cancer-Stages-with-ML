# Breast Cancer Classification using Machine Learning

This project applies multiple supervised learning models to classify breast cancer instances as **benign (2)** or **malignant (4)** using the **Wisconsin Breast Cancer Dataset**. The models are evaluated based on accuracy, precision, recall, and advanced performance curves (ROC & Precision-Recall).

---

## Dataset

- **Source**: [UCI Machine Learning Repository - Breast Cancer Wisconsin (Diagnostic)](https://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+(original))
- **Features**: 9 input features + 1 target variable
- **Target Classes**:
  - `2` → Benign
  - `4` → Malignant

---

## Technologies Used

- Python
- Scikit-learn
- Pandas
- NumPy
- Seaborn / Matplotlib

---

## Models Applied

- **Logistic Regression**
- **Support Vector Machine (RBF Kernel)**
- **Random Forest Classifier**

Data balancing was done using **SMOTE (Synthetic Minority Over-sampling Technique)** to handle class imbalance before training.

---

## Model Evaluation

### Accuracy Scores:

| Model                | Accuracy |
|---------------------|----------|
| Logistic Regression | 96.67%   |
| SVM (RBF Kernel)    | 97.62%   |
| Random Forest       | 97.14%   |

---

### ROC Curve (AUC Scores):

| Model                | AUC Score |
|---------------------|-----------|
| Logistic Regression | 1.00      |
| SVM (RBF Kernel)    | 0.99      |
| Random Forest       | 1.00      |

---

### Confusion Matrix (Sample - Logistic Regression):
          Predicted
         |   2 |  4
     ---------------
  2  |  141 |  2
  4  |   5  | 62

---

## Key Insights

- SMOTE significantly improved class balance and overall model performance.
- All models achieved **very high AUC scores (≥ 0.99)**, indicating excellent classification ability.
- Logistic Regression and Random Forest achieved **perfect or near-perfect separation**, suggesting potential overfitting — validated with confusion matrix.
- SVM, while slightly lower, still offers **strong generalization and robustness**.

---

## How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/breast-cancer-classification.git
   cd breast-cancer-classification
