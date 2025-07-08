# 🚢 Titanic Survival Prediction - Machine Learning Project

This project aims to predict whether a passenger survived the Titanic disaster using supervised machine learning. It uses the Titanic dataset, performing data preprocessing, exploratory data analysis (EDA), feature engineering, and logistic regression for classification.

---

## 📌 Project Structure

- `Step 1:` Import necessary libraries  
- `Step 2:` Read dataset  
- `Step 3:` Quick data audit  
- `Step 4:` EDA  
- `Step 5:` Handling missing values  
- `Step 6:` Outliers treatment 
- `Step 7:` Treat duplicates & garbage values  
- `Step 8:` Encoding of data
- `Step 9:` Model Training and Evaluation  

---

## 📊 Dataset Information

Features used:
- `pclass` - Passenger class (1st, 2nd, 3rd)
- `sex` - Gender
- `age` - Age in years
- `sibsp` - Siblings/spouses aboard
- `parch` - Parents/children aboard
- `fare` - Ticket fare
- `embarked`, `class`, `who`, `embark_town`, `alive`, `alone` - Categorical features encoded

Target:
- `survived` (0 = No, 1 = Yes)

---

## 🧹 Preprocessing Steps

- Removed duplicates
- Handled missing values:
  - Numeric: filled with median
  - Categorical: filled with mode
- Detected and capped outliers using IQR method
- Encoded categorical variables using `pd.get_dummies()`

---

## 🤖 Model Used

- **Logistic Regression** (scikit-learn)
- Accuracy Achieved: **100%** (may be subject to overfitting or data leakage — under validation)

Evaluation metrics:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

---

## 📦 Dependencies

```bash
pandas
numpy
matplotlib
seaborn
scikit-learn
