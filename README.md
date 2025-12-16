# Breast Cancer Classification using Logistic Regression

This project demonstrates a **binary classification model** to predict **malignant vs benign breast tumors** using the **Breast Cancer Wisconsin dataset**. The goal was not only to achieve high accuracy but also to emphasize **proper feature selection, preprocessing, and evaluation metrics** for medical applications.

---

## 📂 Dataset

- Source: [UCI ML Repository / Kaggle](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data)
- Features: 30 numeric features describing cell nuclei (mean, SE, worst)
- Target: `diagnosis` (Malignant `M` / Benign `B`)

---

## 🛠️ Approach

1. **Exploratory Data Analysis**
   - Checked correlations
   - Removed highly collinear features to improve interpretability

2. **Preprocessing**
   - Converted target `M`/`B` → `1`/`0`
   - Train-test split **before scaling** to prevent data leakage
   - StandardScaler applied via **Pipeline**

3. **Model**
   - Logistic Regression
   - Trained on selected numeric features
   - Evaluation metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC, Confusion Matrix

---

## 📊 Results

**Test Set Metrics**:  

- Accuracy: ~0.982  
- Precision: 1.0  
- Recall: 0.953  
- F1-score: 0.976  
- ROC-AUC: 0.997  

**Interpretation:**  
- 0 false positives (all predicted malignant cases were correct)  
- 2 false negatives (2 malignant cases missed)  
- Model generalizes well, minimal overfitting observed

---

## 📈 Visualizations

<img width="680" height="565" alt="image" src="https://github.com/user-attachments/assets/20666d72-8a6c-48a4-a0d6-e3f9aff791ba" />
<img width="273" height="343" alt="image" src="https://github.com/user-attachments/assets/6b62c0b1-624a-4a39-ad57-fbb4a2d42801" />


---

## 🔑 Key Takeaways

- Proper feature selection and avoiding data leakage is crucial for medical datasets  
- Evaluation metrics like **recall and ROC-AUC** are more meaningful than raw accuracy  
- Logistic Regression can be highly effective for linearly separable medical data  

---

## 📂 How to run

1. Clone this repository:  
```bash
git clone https://github.com/Yokaiiiii/breast-cancer-prediction.git
```
2. Open the notebook in Google Colab or Jupyter

3. Run all cells to reproduce results

## 🔗 References

- Breast Cancer Wisconsin (Diagnostic) Data Set - Kaggle

- Scikit-learn Logistic Regression

🚀 Author

Rujan Bastola

- LinkedIn: linkedin.com/in/rujanbastola/

- Machine Learning Enthusiast
