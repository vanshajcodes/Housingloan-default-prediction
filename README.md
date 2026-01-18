# Credit Risk PD Modeling (End-to-End) 

## 📌 Project Overview

This project demonstrates an **end-to-end credit risk modeling pipeline**, starting from **Probability of Default (PD) estimation** and extending to **credit scorecard development**. The workflow is designed to closely mirror **industry and regulatory practices used in banks**, with a strong focus on **interpretability, validation, and governance**.

The project is intentionally built using **logistic regression**, reflecting its widespread acceptance in **credit risk modeling and model validation environments**.

---

## 🎯 Objectives

* Build an interpretable **PD model** for retail credit risk using logistic regression
* Evaluate model performance using **bank-standard metrics** (AUC, Gini, KS)
* Improve probability accuracy through **calibration techniques**
* Convert calibrated PDs into a **production-style credit scorecard** using log-odds and PDO scaling
* Demonstrate a **clear linkage** between statistical modeling outputs and business decisioning

---

## 📂 Dataset

* **Home Credit Default Risk Dataset** (Kaggle)
* Target variable: `TARGET` (1 = Default, 0 = Non-default)
* Features include demographic, financial, and behavioral variables

> ⚠️ Note: This project uses publicly available data. No proprietary or bank data is included.

---

## 🧠 Methodology

### 1️⃣ Data Preparation & Exploration

* Missing value treatment (median / mode imputation)
* Categorical variable encoding
* Feature scaling for numerical stability
* Train / validation data split

### 2️⃣ PD Model Development

* **Logistic Regression** with L1/L2 regularization
* Regularization used to control overfitting and improve stability
* Model trained to estimate borrower-level **Probability of Default (PD)**

### 3️⃣ Model Evaluation (Discrimination)

* **ROC-AUC** – ranking power
* **Gini Coefficient** – normalized discriminatory strength
* **KS Statistic** – separation between default and non-default populations

### 4️⃣ Probability Calibration

* Calibration curves to assess probability accuracy
* **Platt Scaling (Sigmoid calibration)** applied
* Brier Score used to compare calibrated vs uncalibrated outputs

> Distinction maintained between **discrimination** and **calibration**, as expected in banking model validation.

## 🛠 Tools & Technologies

* **Python**: pandas, numpy, scikit-learn
* **Modeling**: Logistic Regression (Regularized)
* **Validation Metrics**: AUC, Gini, KS, Brier Score
* **Visualization**: matplotlib

---

## 📌 Key Learning Outcomes

* Practical understanding of **PD modeling in a banking context**
* Hands-on exposure to **model validation metrics and calibration**
* Clear separation of **model development** and **business decision layers**
* Experience with **scorecard construction aligned with industry standards**

---

## 🧩 Governance & Disclaimer

This project is intended for **educational and demonstration purposes only**. It does not represent a production or regulatory-approved model. Methodology and validation steps are aligned with commonly used practices in **credit risk analytics and model validation teams**.

---

## 👤 Author

**Vanshaj, FRM**
Credit Risk & Model Validation Enthusiast

---

Contact

For discussions related to credit risk modeling, validation, or analytics roles, feel free to connect via LinkedIn or GitHub.
