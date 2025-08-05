# 🧠 Drug Type Prediction - Memory Test on Drugged Islanders

This project involves classifying the type of drug administered to individuals based on memory test data. We evaluate a range of machine learning models to identify the most effective approach for this multi-class classification problem.

## 📂 Dataset

- **Source**: [Kaggle - Memory Test on Drugged Islanders](https://www.kaggle.com/datasets/steveahn/memory-test-on-drugged-islanders-data)
- **Description**: Features include demographic and test-based information. The target variable indicates the drug type.
- **Classes**: 3 drug categories (encoded as `0`, `1`, `2`)

---

## 🧪 Preprocessing

- **Encoding**:
  - Categorical features were processed using:
    - `Label Encoding` for ordinal variables
    - `OneHot Encoding` for nominal variables
- **Feature Scaling**:
  - `StandardScaler` was applied to normalize the data before model training.

---

## 🔍 Models Evaluated

| Model                                | Accuracy |
|-------------------------------------|----------|
| Logistic Regression                 | 40.00%   |
| K-Nearest Neighbors (KNN)           | 35.00%   |
| Decision Tree                       | 40.00%   |
| SVM (Linear Kernel)                 | 35.00%   |
| SVM (RBF Kernel)                    | 45.00%   |
| Neural Network                      | 37.50%   |
| Random Forest                       | 45.00%   |
| Gradient Boosting                   | **55.00%** ✅ |
| XGBoost                             | 40.00%   |
| LightGBM                            | 40.00%   |
| CatBoost                            | 47.50%   |

> 🎯 **Best Model**: Gradient Boosting with an accuracy of **55.00%**

---

## 📊 Evaluation Metrics

### ✅ Confusion Matrix

| Actual \ Predicted | A | T | S |
|--------------------|---|---|---|
| **A**              | 7 | 2 | 3 |
| **T**              | 3 | 7 | 5 |
| **S**              | 2 | 3 | 8 |


### 📄 Classification Report:
| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.58      | 0.58   | 0.58     | 12      |
| 1     | 0.58      | 0.47   | 0.52     | 15      |
| 2     | 0.50      | 0.62   | 0.55     | 13      |

- **Macro Avg F1-Score**: 0.55
- **Weighted Avg F1-Score**: 0.55
- **Overall Accuracy**: 55%

---

## 🛠️ Tools & Libraries

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost, LightGBM, CatBoost
- Matplotlib, Seaborn

---

## 📌 How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/BrijeshRakhasiya/Drug-Type-Prediction.git
   cd drug-type-prediction


# 🙋‍♂️ Author
Brijesh Rakhasiya
AI/ML Enthusiast | Data Scientist | Problem Solver


## 📄 License

This project is licensed under the MIT License.

---
**Made ❤️ by Brijesh Rakhasiya**
