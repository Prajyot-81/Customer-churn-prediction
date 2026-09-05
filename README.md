Customer Churn Prediction 📊

An end-to-end Machine Learning project that predicts whether a telecom customer is likely to churn using Python, Scikit-learn, XGBoost, SHAP, and Streamlit.

• Project Overview

Customer churn is a major challenge for telecom companies. The goal of this project is to identify customers who are likely to leave the company so that businesses can take proactive retention actions.

This project covers the complete Machine Learning workflow:

Data Cleaning → EDA → Feature Engineering → Preprocessing → Model Training → Hyperparameter Tuning → Model Evaluation → Explainable AI → Streamlit Deployment

• Dataset

The project uses the IBM Telco Customer Churn Dataset.

- Rows: 7,043
- Features: 20
- Target: Churn
- Churn Classes: "Yes / No"

• Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- SHAP
- Streamlit
- Jupyter Notebook
- Git & GitHub

• Exploratory Data Analysis

The project analyzes important customer characteristics such as:

- Contract type
- Monthly charges
- Tenure
- Customer services
- Payment methods
- Internet service
- Churn distribution

• Machine Learning Models

Multiple classification models were evaluated:

- Logistic Regression
- Random Forest
- XGBoost

XGBoost was selected as the final model and further improved using RandomizedSearchCV.

• Model Performance

Final tuned XGBoost model:

Metric| Score
Accuracy| 80.70%
ROC-AUC| 84.77%
Churn Recall| 50.27%
Churn F1-Score| 58.02%

Best hyperparameters:

n_estimators = 300
max_depth = 4
learning_rate = 0.01
subsample = 0.8

• Explainable AI — SHAP

SHAP (SHapley Additive exPlanations) was used to understand which features have the greatest influence on customer churn predictions.

This helps make the Machine Learning model more interpretable and useful for business decision-making.

• Streamlit Application

The project includes an interactive Streamlit application where users can enter customer information and receive:

- Churn prediction
- Churn probability
- Customer retention insight

Run the application

streamlit run app.py

• Project Structure

Customer-Churn-Prediction/
│
├── app.py
├── best_model.pkl
├── preprocessor.pkl
│
├── data/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── contract_churn.png
├── monthlycharges_churn.png
├── tenure_churn.png
├── shap_summary.png
│
├── .gitignore
└── README.md

• Business Insights

The model can help telecom companies:

- Identify high-risk customers
- Prioritize retention campaigns
- Understand major churn drivers
- Reduce customer acquisition costs
- Improve customer retention strategies

• Future Improvements

- Handle class imbalance using SMOTE or class weights
- Optimize the classification threshold for better churn recall
- Add a customer segmentation module
- Add Power BI dashboard
- Deploy the application online
- Add real-time prediction API

• Author

Prajyot Bande

BSc Computer Science | Data Science & Machine Learning

• Skills

Python • Machine Learning • SQL • Data Analysis • XGBoost • SHAP • Streamlit

---

If you find this project useful, consider giving the repository a star!
