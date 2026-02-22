# 📊 Handling Imbalanced Data using SMOTE & Oversampling

## 📌 Project Overview
This project demonstrates how to handle **severely imbalanced datasets** using **SMOTE (Synthetic Minority Over-sampling Technique)**.

The dataset suffers from extreme class imbalance, where the majority class dominates the minority class, leading to misleading model accuracy.

---

## 📂 Dataset Description

- Binary Classification Problem
- Target Classes: 0 and 1
- Class Distribution:
  - Class 0 → 99.8%
  - Class 1 → 0.2%
- Severe imbalance causing model bias

Such imbalance results in:
- High overall accuracy
- Poor minority class detection
- Biased predictions toward majority class

---

## 🚨 Problem: Why Oversampling Was Needed

From the confusion matrix:

- True Negatives: 85284
- False Positives: 12
- False Negatives: 56
- True Positives: 91

Even though accuracy appears extremely high, the dataset is dominated by Class 0.  
The minority class (Class 1) is underrepresented and easily misclassified.

Because:

- 99.8% of the data belongs to Class 0
- Only 0.2% belongs to Class 1
- The model tends to predict Class 0 most of the time

This creates a **biased model**.

To solve this issue, **SMOTE** was applied to synthetically generate new minority class samples.

---

## 📊 Model Evaluation Before Oversampling

### Confusion Matrix

<img width="720" height="533" alt="Screenshot 2026-02-22 235459" src="https://github.com/user-attachments/assets/1fb1972b-9c91-4440-b3fe-b673b535262e" />


The confusion matrix shows:
- Strong bias toward Class 0
- Minority class misclassification
- Misleading high accuracy

---

### Class Distribution

<img width="549" height="439" alt="Screenshot 2026-02-22 235441" src="https://github.com/user-attachments/assets/6c2906ad-e61a-4a23-9e8e-e3afe70700f8" />


The dataset is extremely imbalanced:
- 99.8% → Class 0
- 0.2% → Class 1

This imbalance justifies the need for oversampling.

---

## 🛠️ Techniques Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Matplotlib / Seaborn

---

## 🔄 Solution Applied

SMOTE was used to:
- Generate synthetic minority samples
- Balance class distribution
- Improve recall for minority class
- Reduce model bias

---

## 📈 Key Learning Outcomes

- Understanding imbalanced datasets
- Why accuracy is misleading in skewed data
- Applying SMOTE for class balancing
- Evaluating models using confusion matrix
- Importance of Recall & F1-score

---

## 🚀 How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn
   ```
3. Run the notebook:
   ```bash
   jupyter notebook Smote_&_Oversampling.ipynb
   ```

---

## 📌 Conclusion

In highly imbalanced datasets, accuracy alone is not a reliable metric.  
Oversampling techniques like SMOTE help create a balanced dataset and improve minority class prediction performance.

---

## 👤 Author
Aditya Uttekar

---

⭐ If you found this helpful, consider giving this repository a star!
