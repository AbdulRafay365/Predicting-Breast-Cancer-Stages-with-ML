# Breast Cancer Classification using Machine Learning
<p align="center">
  <img src="https://github.com/user-attachments/assets/21df4f2b-7be3-4b13-8871-d54588bfb5a5" alt="1430540" />
</p>

## Overview
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

## Key Insights

- SMOTE significantly improved class balance and overall model performance.
- All models achieved **very high AUC scores (≥ 0.99)**, indicating excellent classification ability.
- Logistic Regression and Random Forest achieved **perfect or near-perfect separation**, suggesting potential overfitting — validated with confusion matrix.
- SVM, while slightly lower, still offers **strong generalization and robustness**.

---

## How to Run

1. **Clone the Repository**  
```bash
git clone https://github.com/AbdulRafay365/Predicting-Breast-Cancer-Stages-with-ML.git
cd Predicting-Breast-Cancer-Stages-with-ML
```

2. **Install Dependencies**
```bash
pip install -r requirements.txt
```

3. Run the notebook in Scripts folder using Google Colab

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
