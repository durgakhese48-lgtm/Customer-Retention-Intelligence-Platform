# Customer Retention Intelligence Platform

An end-to-end **Customer Churn Prediction** application that identifies at-risk customers and explains *why* they're likely to churn — helping businesses take proactive retention action.

**Duration:** Dec 08, 2025 – Jan 02, 2026  
**Team Size:** 2

---

## 🚀 Overview

This project builds a full machine learning pipeline — from raw data to an interactive dashboard — to predict customer churn and surface the key drivers behind each prediction using Explainable AI (SHAP).

**Key capabilities:**
- Cleaned and preprocessed raw customer data for modeling
- Engineered features to capture behavioral and usage signals
- Balanced classes using **SMOTE** to handle churn-label imbalance
- Trained and evaluated multiple ML models (Logistic Regression, Random Forest, XGBoost)
- Generated **SHAP** explainability plots for individual and global predictions
- Built an interactive **Streamlit** dashboard for business users to explore churn risk and drivers
- Deployed-ready setup on **AWS**

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Data Handling | SQL, Pandas |
| ML / Modeling | Scikit-learn, XGBoost |
| Class Balancing | SMOTE (imbalanced-learn) |
| Explainability | SHAP |
| Dashboard | Streamlit |
| Version Control | Git |
| Deployment/Infra | AWS |
| Monitoring | Model performance & drift monitoring |

---

## 📁 Project Structure

```
customer-retention-intelligence-platform/
├── data/
│   ├── raw/                # Original, unprocessed data
│   └── processed/          # Cleaned & feature-engineered data
├── notebooks/               # EDA and experimentation notebooks
├── src/                      # Core source code
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── train_model.py
│   ├── evaluate_model.py
│   └── explain_model.py      # SHAP explainability
├── app/
│   └── streamlit_app.py      # Interactive dashboard
├── models/                    # Saved/serialized trained models
├── reports/
│   └── figures/               # SHAP plots, model evaluation charts
├── requirements.txt
├── .gitignore
└── README.md
```

---

## ⚙️ Setup & Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/customer-retention-intelligence-platform.git
   cd customer-retention-intelligence-platform
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Streamlit dashboard**
   ```bash
   streamlit run app/streamlit_app.py
   ```

---

## 🧠 Approach

1. **Data Preprocessing** — Handled missing values, encoded categorical variables, and cleaned inconsistencies in raw customer data.
2. **Feature Engineering** — Derived behavioral and usage-based features to improve model signal.
3. **Class Imbalance Handling** — Applied SMOTE to oversample the minority (churn) class for fairer model training.
4. **Model Training & Evaluation** — Trained Logistic Regression, Random Forest, and XGBoost models; compared performance using metrics like accuracy, precision, recall, F1, and ROC-AUC.
5. **Explainable AI** — Used SHAP to interpret model predictions at both global (feature importance) and local (individual customer) levels.
6. **Dashboard** — Built an interactive Streamlit app so business stakeholders can explore churn risk scores and drivers without needing to read code.

---

## 📊 Results

> _Add your final model performance metrics here, e.g.:_
- Best Model: XGBoost
- Accuracy: __%
- Precision / Recall: __ / __
- ROC-AUC: __

---

## 📌 Future Improvements

- Automate model retraining pipeline
- Add real-time monitoring for data/model drift
- Deploy dashboard publicly via AWS (e.g., EC2 / Elastic Beanstalk)

---

## 👥 Contributors

- Your Name — [GitHub](https://github.com/<your-username>)
- Teammate Name — [GitHub](https://github.com/<teammate-username>)

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
