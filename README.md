# Credit-Risk-Profiler
![Credit-Risl=Wallpaper](bank_interest_wallpaper.jpg)

An end-to-end machine learning pipeline that predicts applicant risk levels—**High**, **Medium**, or **Low**—based on financial behavior and credit patterns. Built using advanced feature engineering, balanced learning, and optimized XGBoost modeling.

---

## 📌 About

This project targets **financial institutions** and **credit analysts** looking to automate and improve loan underwriting processes. By classifying applicants based on risk, it minimizes default rates, improves portfolio quality, and supports data-driven lending decisions.

---

## 🔍 Business Insights

The project provides real, actionable insights to inform lending strategies:

![Risk_distribution_img](risk_distribution_img.png")

- 💡 **High Risk (38.4%)** – Applicants in this group may pose a default threat and should undergo stringent manual review or be offered secured credit products with collateral.
- 💡 **Medium Risk (36.5%)** – Moderate-risk customers can be extended limited credit or subject to stricter repayment terms.
- 💡 **Low Risk (25.1%)** – Safe borrowers ideal for fast-tracking, loyalty offers, or upselling.

By visually mapping financial behavior to risk categories, the model empowers lenders to:

- 📉 Reduce non-performing loans (NPLs)
- 📊 Optimize interest rates and credit limits
- 🧠 Make data-informed decisions across the credit lifecycle

---

## 📊 Risk Profiling (Core Strategy)

Credit risk profiling enables segmentation of loan applicants based on behavioral and financial data. The model evaluates:

- 📌 Credit utilization stress
- 📌 Delinquency and repayment patterns
- 📌 Debt-to-income vs. loan-to-income dynamics
- 📌 Number of active/open accounts
- 📌 Income vs. exposure normalization

### 📈 Sample Risk Distribution (Pie Chart Output)
| Risk Level   | Distribution |
|--------------|--------------|
| High Risk    | 38.4%        |
| Medium Risk  | 36.5%        |
| Low Risk     | 25.1%        |

---

## 🚀 Key Features

- ✅ Custom Feature Engineering based on credit behavior
- ✅ Class imbalance resolved using SMOTETomek
- ✅ XGBoost modeling with GridSearchCV hyperparameter tuning
- ✅ Insightful visual analytics (risk distribution, metrics table, feature impact)
- ✅ Production-ready modular code
- ✅ Business-focused segmentation (bins, ratios, and derived flags)

---

## ⚙️ Custom Feature Engineering Summary

| Feature Name             | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `Debt_Income_Ratio`      | Ratio of debt burden to income-adjusted loan size                          |
| `Income_per_Account`     | Measures income efficiency across credit lines                             |
| `Delinq_Ratio`           | Tracks delinquencies per active account                                    |
| `Credit_Utilization`     | Loan request vs. income (credit stress proxy)                              |
| `Open_Account_Rate`      | Proportion of open accounts to all accounts                                |
| `Loan_to_Income_Bin`     | Risk groupings based on loan-to-income ratio                               |
| `Log_Income_Bin`         | Segments applicants into income tiers using quantiles                      |

These features drive model interpretability and improve predictive strength by embedding domain logic.

---

## 📂 Folder Structure

```

📦 Credit-Risk-Profiler-XGBoost/
├── data/                  # Raw and processed datasets
├── notebooks/             # EDA, training, tuning, visualization
├── outputs/               # Saved charts, reports, tables
├── models/                # Trained models, metrics
├── src/                   # Feature engineering, utils, modeling scripts
├── risk\_prediction.py     # Main script for running pipeline
├── requirements.txt       # Dependencies
└── README.md              # Documentation

````

---

## 📈 Model Performance

| Metric     | Score   |
|------------|---------|
| Accuracy   | 88.5%   |
| F1-Score   | 0.87    |
| ROC-AUC    | 0.91    |


---

## 🛠 Tech Stack

- **Language**: Python
- **Core Libraries**:  
  `pandas`, `numpy`, `scikit-learn`, `xgboost`, `imblearn`, `seaborn`, `matplotlib`, `plotly`
- **Modeling**: XGBoost
- **Hyperparameter Tuning**: GridSearchCV
- **Deployment Ready**: Modular scripts, CLI runnable

---

## 📊 Visual Insights

- 📌 **Overall Risk Distribution (Pie Chart)**  
- 📌 **Risk vs. Employment Length**  
- 📌 **Delinquency Patterns by Risk Group**  
- 📌 **Financial Metric Summary Table by Risk Category**  
- 📌 **Loan Purpose vs Risk Category**

---

## ✅ How to Run

```bash
# 1. Clone the Repository
git clone https://github.com/your-username/Credit-Risk-Profiler-XGBoost.git
cd Credit-Risk-Profiler-XGBoost

# 2. Install Dependencies
pip install -r requirements.txt

# 3. Run the Main Script
python risk_prediction.py
````

---

## 🧭 Future Enhancements

* 🌐 Streamlit or Dash web interface for business users
* ⚙️ REST API using Flask or FastAPI
* 📊 Explainability using SHAP values
* 💾 Cloud storage integration (AWS S3, GCP)

---

## 📜 License

This project is licensed under the **Apache License** – open to use and contribute.

---

## 👤 Author

**Shreya Pandey**
📫 [LinkedIn](https://www.linkedin.com/in/shreya-pandey-97252431b/)

---
