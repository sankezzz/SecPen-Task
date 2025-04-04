# 🛡️ Network Intrusion Detection Using Machine Learning  

This project aims to detect network intrusions using machine learning models, including **Random Forest** and a **Basic Artificial Neural Network (ANN)**. It utilizes the **CICIDS2017 dataset** for classification of network traffic into "Normal" or "Attack" categories.  

---

## 🚀 **Features**  

✅ Preprocessing of network traffic data (handling missing values, normalization, encoding)  
✅ Feature selection based on correlation and importance  
✅ Model training with **Random Forest** and **ANN**  
✅ Evaluation using precision, recall, f1-score, and accuracy  
✅ **Visualization:** Confusion Matrix, Feature Importance, ROC Curve, and Heatmap  

---

## 🛠 **Setup Instructions**  

### 1️⃣ Install Dependencies  
Ensure you have Python installed, then install required packages using:  

```bash
pip install -r requirements.txt
```  

### 2️⃣ Run the Model Training Script  
Run the ipynb file cell by cell to execute the code

---  

## 📊 **Data Preprocessing**  

1. **Handling Missing Values:**  
   - Identified missing values in categorical and numerical features.  
   - Removed non-essential columns such as timestamps and text-based fields.  
   - Replaced missing numerical values with column mean/median.  

2. **Feature Selection Using Correlation Analysis:**  
   - Dropped irrelevant columns (e.g., timestamps, textual features).  
   - Selected highly correlated features for better model performance.  

---  

## 🤖 **Model Training & Evaluation**  

We trained two machine learning models:  

### 1️⃣ **Random Forest Classifier**  

📌 **Classification Report:**  

| Class   | Precision | Recall | F1-score | Support |
|---------|-----------|--------|----------|---------|
| Attack  | 0.98      | 0.97   | 0.98     | 755     |
| Normal  | 1.00      | 1.00   | 1.00     | 33521   |

✅ **Random Forest Accuracy:** **99.91%**  

📌 **Confusion Matrix:**  
![Confusion Matrix - Random Forest](confusion_matrix_rf.png)  

📌 **Feature Importance:**  
![Feature Importance](feature_importance.png)  

---  

### 2️⃣ **Artificial Neural Network (ANN)**  

📌 **Classification Report:**  

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.94      | 0.33   | 0.49     | 755     |
| 1     | 0.99      | 1.00   | 0.99     | 33521   |

✅ **ANN Accuracy:** **98.0%**  

📌 **Confusion Matrix:**  
![Confusion Matrix - ANN](confusion_matrix_ann.png)  

📌 **ROC Curve:**  
![ROC Curve](roc_curve.png)  

---  

## 📈 **Results & Observations**  

- **Random Forest** performed better with **higher accuracy and F1-score**, making it more reliable for intrusion detection.  
- **ANN had lower recall for the "Attack" class**, meaning it missed more attack cases than Random Forest.  
- Feature importance analysis revealed key features that contribute to classification decisions.  

---  

## 📌 **Conclusion**  

This project successfully demonstrates network intrusion detection using **Random Forest** and **ANN**. The **Random Forest model outperforms ANN**, making it a more suitable choice for real-world implementation.  

---  

## 📜 **License**  

This project is open-source and available under the MIT License.  

---  

🔹 **Developed by:** Sanket Suryawanshi  
