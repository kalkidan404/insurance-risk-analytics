# Insurance Risk Analytics & Pricing Model

## 📌 Project Overview

This project builds a data-driven insurance risk analytics system that predicts:

- The probability of an insurance claim
- The expected claim severity
- A risk-based premium pricing model

The goal is to improve underwriting decisions using machine learning and explainable AI techniques.

---

## 📂 Project Structure

```

insurance-risk-analytics/
│
├── data/                  # Raw and processed datasets (DVC managed)
├── notebooks/             # Jupyter notebooks for EDA and modeling
├── src/                   # Modular Python source code
│   ├── data/              # Data loading & preprocessing
│   ├── features/          # Feature engineering
│   ├── models/            # Training, evaluation, prediction
│   ├── analysis/          # EDA and hypothesis testing
│   └── utils/             # Helper functions
│
├── reports/               # Final report and figures
├── dvc.yaml               # Data pipeline tracking
├── requirements.txt       # Dependencies
├── setup.py               # Package setup
└── README.md              # Project documentation

```

---

## ⚙️ Workflow

### 1. Data Understanding & EDA

- Data cleaning and preprocessing
- Exploratory analysis of claims and premiums
- Loss ratio analysis by province, vehicle type, and gender

### 2. Feature Engineering

- Creation of key features such as:
  - Vehicle Age
  - Loss Ratio
  - Margin
  - Claim indicator (HasClaim)

### 3. Modeling

#### 🧠 Model 1: Claim Prediction (Classification)

- Algorithm: Random Forest Classifier
- Output: Probability of claim occurrence

#### 💰 Model 2: Claim Severity (Regression)

- Algorithm: Random Forest Regressor
- Output: Expected claim amount

#### 💸 Pricing Model

Final premium calculated using:

\[
\text{Suggested Premium} =
(\text{Claim Probability} \times \text{Expected Severity}) + Base + Risk Adjustment
\]

---

## 📊 Explainability (SHAP)

SHAP (SHapley Additive exPlanations) was used to interpret model decisions.

Key insights:

- Vehicle characteristics strongly influence claim risk
- Higher insured values increase expected claim severity
- Geographic and demographic factors affect risk distribution

---

## 📈 Key Results

- Built predictive model for insurance claims
- Developed risk-based pricing engine
- Identified major risk drivers using SHAP
- Improved transparency in underwriting decisions

---

## 🛠️ Technologies Used

- Python
- Pandas & NumPy
- Scikit-learn
- SHAP
- Matplotlib & Seaborn
- DVC (Data Version Control)
- Git & GitHub

---

## 🚀 How to Run

### 1. Clone repository

```bash
git clone https://github.com/your-username/insurance-risk-analytics.git
cd insurance-risk-analytics
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run notebooks

Open Jupyter Notebook and run:

```
notebooks/05_modeling.ipynb
```

---

## 📌 Notes

- Large dataset is managed using DVC
- Models are trained on sampled data for performance
- SHAP analysis uses a subset of data for efficiency

---

## 📎 Future Improvements

- Hyperparameter tuning for models
- Deployment as an API (FastAPI/Flask)
- Real-time premium calculator
- Advanced explainability dashboards

---

## 👤 Author

Insurance Risk Analytics Project
