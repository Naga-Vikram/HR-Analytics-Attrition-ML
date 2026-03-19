# 🤖 HR Analytics – Employee Attrition Prediction (Machine Learning)

## 🎯 Objective

This project extends HR attrition analysis into predictive modeling, aiming to identify employees at risk of leaving and uncover the key drivers influencing attrition.

The goal is not just prediction, but business-oriented interpretation of model outputs to support workforce retention strategies.

---
## 🗂️ Dataset

- **Original Source:** [IBM HR Analytics Employee Attrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Database Storage:** PostgreSQL database hosted on Supabase
- **Access Method:** Data was extracted from Supabase and used as a CSV file for analysis
- **File Included:** `data/HR_Attrition_Data.csv`
- **Records:** 1,470 employees
- **Kaggle Notebook:** [HR-Analytics-Attrition-ML](https://www.kaggle.com/code/vikky11/hr-analytics-mlmodel)

---

## 🧠 Models Implemented

- Logistic Regression  
- Random Forest  
- XGBoost  

---

## 📊 Model Performance Comparison

| Model | Accuracy | Precision | Recall | F1 Score |
|------|--------|----------|--------|--------|
| Logistic Regression | 0.73 | 0.33 | **0.59** | 0.42 |
| Random Forest | **0.81** | 0.39 | 0.25 | 0.31 |
| XGBoost | 0.78 | 0.35 | 0.47 | 0.40 |

---

## 🔍 Key Insight: Accuracy vs Recall

While Random Forest achieved the highest accuracy, it failed to identify employees who are likely to leave (low recall).

👉 In HR analytics, **Recall is more important than Accuracy**, because:

- Missing a leaving employee = high business cost  
- False alarms are acceptable, but missed attrition is not  

---

## 🏆 Model Selection

- ✅ **Best Business Model:** Logistic Regression (highest recall)  
- ⚖️ **Best Balanced Model:** XGBoost  
- 📉 **Not Recommended Alone:** Random Forest (misses attrition cases)  

---

## 📉 Confusion Matrix Comparison

### Logistic Regression
[[189 58]  
[ 19 28]]


### Random Forest
[[228 19]  
[ 35 12]]

### XGBoost


[[206 41]  
[ 25 22]]


---

## 📊 Key Drivers of Attrition

Across models, consistent factors influencing attrition include:

### 🔥 High Risk Factors

- Overtime (strongest driver)  
- Sales & HR departments  
- Laboratory Technician role  

### 🔻 Retention Factors

- Higher monthly income  
- Longer tenure (years at company)  
- Increased age and experience  

---

## 📈 Model Interpretation

### Logistic Regression

- Provides clear directional insights (positive/negative impact)  
- Highly interpretable for business stakeholders
<img width="1019" height="527" alt="image" src="https://github.com/user-attachments/assets/02eb1a33-6f1d-4271-ae0f-aa5154d5c567" />


### Random Forest

- Captures complex relationships  
- Less interpretable but useful for feature importance
<img width="1025" height="547" alt="image" src="https://github.com/user-attachments/assets/df8b3fc9-4f29-44ab-8e37-b7159647fef9" />


### XGBoost

- Strong performance with balanced precision and recall  
- Effective for production-level models
<img width="1027" height="550" alt="image" src="https://github.com/user-attachments/assets/b033577f-44da-4676-8137-e35b11504d2e" />


---

## 🧠 Business Takeaways

- Employees working overtime are significantly more likely to leave  
- Early-career employees show higher attrition risk  
- Compensation plays a key role in retention  
- Certain job roles consistently exhibit higher turnover  

---

## 🚀 Project Value

This project demonstrates:

- 🔄 End-to-end analytics workflow (SQL → Excel → Power BI → ML)  
- 📊 Ability to translate business problems into predictive models  
- 🧠 Model evaluation based on business impact, not just accuracy  
- 📈 Insight-driven interpretation of machine learning outputs  

---

## 📁 Files Included

- `attrition_model.ipynb` → ML implementation
- `data/` → dataset  
  
---

## 🔗 Related Projects

- [Excel Dashboard (HR Analytics)](https://github.com/Naga-Vikram/HR-Analytics-Employee-Attrition-Excel) 
- [Power BI Dashboard (HR Attrition Analysis)](https://github.com/Naga-Vikram/HR-Analytics-PowerBI-Attrition) 

---



## ✅ Conclusion

This project shows how machine learning can move beyond prediction and become a **decision-support tool** in HR analytics.


