##  Churn Prediction Project

## 🔎 Overview
This project predicts **customer churn** using machine learning models. 
Churn prediction helps businesses identify customers likely to leave, enabling proactive retention strategies.

## 📂 Repository Structure
- `data/` → Dataset file(.csv) 
- `notebooks/` →  notebooks for exploration & modeling(.ipynb)
- `models/` → Saved models (`.pkl`)  
- `app/` → Streamlit app for deployment  
- `README.md` → Project documentation  

---

## ⚙️ Workflow
1. **Data Preprocessing**
   - Handle missing values  
   - Encode categorical variables (e.g., gender)  
   - Scale numerical features (age, tenure, charges)  

2. **Model Training**
   - Algorithms tested: Logistic Regression, KNN, Random Forest, SVM, Decision Tree  
   - Hyperparameter tuning with **GridSearchCV**  
   - Class imbalance handled with **class weights**  

3. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1‑score, ROC‑AUC  
   - Focus on **recall for churners** (catching customers likely to leave)  
   - Compared performance across models  

4. **Deployment**
   - Models saved with `joblib` (`model.pkl`, `scaler.pkl`)  
   - Streamlit app built for interactive predictions  
   - User inputs → scaled → model prediction → churn result displayed  

---

## 📊 Results
- **Logistic Regression**: Best balance (ROC‑AUC ~0.74, recall for both classes reasonable)  
- **KNN, Random Forest, SVM**: High accuracy but biased toward churners  
- **Decision Tree**: Good accuracy, interpretable, moderate balance  

---

## 🚀 Streamlit App
- Input: Age, Gender, Tenure, Monthly Charges  
- Output: Churn prediction (Yes/No)  
- Enhancements: Probability scores, feature importance visualization  

---

## 📈 Key Concepts
- **Accuracy**: Overall correctness of predictions  
- **Precision**: How many predicted churners are actual churners  
- **Recall**: How many actual churners were correctly identified  
- **F1‑score**: Balance between precision & recall  
- **ROC‑AUC**: Ability to separate churners vs non‑churners  

---

If you have suggestions or how can I improve this, lets' connect:
✉️ dishabpps@gmail.com


