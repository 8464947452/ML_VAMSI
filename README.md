
# 📞 Telecom Churn Prediction with LightGBM  

## 📌 **Project Overview**  
This project demonstrates how to predict telecom customer churn using **LightGBM**—a fast and highly efficient gradient boosting framework. Churn prediction is critical for telecom companies to reduce customer attrition, enhance customer retention strategies, and improve profitability.  

The project involves building a LightGBM classifier to predict customer churn based on demographic, service, and account information. The model is trained and evaluated with comprehensive hyperparameter tuning, and detailed insights are derived from advanced visualizations and SHAP analysis.  

---

## 🎯 **Objectives**  
✅ Develop a predictive model using LightGBM to classify telecom customer churn.  
✅ Optimize model performance through hyperparameter tuning using **GridSearchCV**.  
✅ Address class imbalance using threshold adjustments and weighting techniques.  
✅ Evaluate model performance using ROC-AUC, classification reports, and confusion matrices.  
✅ Provide interpretability using SHAP values and feature importance.  

---

## 📂 **Dataset Overview**  
- **Dataset:** Telecom Churn Dataset  
- **Training Samples:** 5,634  
- **Test Samples:** 1,409  
- **Total Features:** 21 (18 categorical + 3 numerical)  

### **Feature Categories**  
| Feature Type | Examples |
|-------------|----------|
| **Numerical** | Tenure, MonthlyCharges, TotalCharges |
| **Categorical** | Contract, PaymentMethod, InternetService, StreamingTV, TechSupport |
| **Target** | Churn (0 = No, 1 = Yes) |  

---

## 🏗️ **Model: LightGBM Classifier**  
LightGBM (Light Gradient Boosting Machine) is a decision-tree-based algorithm that uses histogram-based training. It is known for its efficiency and ability to handle large datasets with categorical and numerical features.

### 🚀 **Why LightGBM?**  
✅ Faster training using histogram-based algorithms.  
✅ Handles categorical features directly without one-hot encoding.  
✅ Supports parallel and GPU-based processing.  
✅ Excellent handling of imbalanced data through cost-sensitive learning.  

---

## 🔧 **Model Training**  
### **Hyperparameter Tuning**  
Hyperparameter tuning was performed using **GridSearchCV** with the following search space:  

| Hyperparameter | Range          | Purpose                                             |
|----------------|----------------|-----------------------------------------------------|
| `num_leaves`   | [31, 50]       | Controls tree complexity                            |
| `max_depth`    | [-1, 10, 20]   | Sets maximum depth (-1 = unlimited)                |
| `learning_rate`| [0.05, 0.1]    | Step size for boosting                             |
| `n_estimators` | [100, 150]     | Number of boosting iterations                      |

## ⚙️ **How to Run the Code**  
### 1. **Clone the Repository**  
```bash
git clone https://github.com/8464947452/ML_VAMSI.git
