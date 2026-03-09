# End-to-End Machine Learning Pipeline for Customer Churn Prediction


## Project Objectives

- Build an **end-to-end ML pipeline** using Scikit-learn Pipeline API  
- Implement **data preprocessing** steps including scaling and encoding  
- Train machine learning models such as **Logistic Regression** and **Random Forest**  
- Perform **hyperparameter tuning using GridSearchCV**  
- Evaluate model performance using appropriate metrics  
- Export the **complete trained pipeline using Joblib** for reuse  

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Joblib
- Matplotlib / Seaborn (for EDA)

---
## Dataset
**Telco Customer Churn Dataset** – includes customer demographics, services, and churn status.

## Approach
1. Load and clean data  
2. Train-test split  
3. Preprocessing pipeline:
   - Numerical → StandardScaler  
   - Categorical → OneHotEncoder  
4. Train models: Logistic Regression & Random Forest  
5. Hyperparameter tuning using **GridSearchCV**  
6. Evaluate model using accuracy & classification report  
7. Export complete pipeline using **Joblib**

## Model Training

The pipeline performs the following steps:

1. Data preprocessing using **ColumnTransformer**
2. Feature scaling using **StandardScaler**
3. Categorical encoding using **OneHotEncoder**
4. Model training using **Logistic Regression** and **Random Forest**
5. Hyperparameter tuning using **GridSearchCV with Cross Validation**

---

## Model Evaluation

The model is evaluated using:

- Accuracy
- Classification Report
- Confusion Matrix

These metrics help assess the model’s performance in predicting customer churn.

---

## Saving the Model

The final trained pipeline is exported using **Joblib** so it can be reused for future predictions.

---

## Conclusion

This project demonstrates how to build a **production-ready, end-to-end machine learning pipeline** for customer churn prediction using the Scikit-learn Pipeline API.  

The pipeline integrates **data preprocessing, feature scaling, encoding, model training, and hyperparameter tuning** into a single workflow, making it **reusable and consistent** for future predictions.  

By exporting the trained pipeline using **Joblib**, it can be **deployed easily** for real-world applications, ensuring reliable predictions while preventing data leakage.  

This notebook and pipeline serve as a **strong foundation for professional ML projects** and can be extended with additional models or deployment strategies.

## Author

**Ume Habiba**  
BS Information Technology Student  
Machine Learning & AI Enthusiast  
Email: umehabiba1088@gmail.com   
LinkedIn: www.linkedin.com/in/ume-habiba-88313537b
