# Credit Card Approval Predictor

A Python-based machine learning project that predicts credit card application approvals by cleaning and imputing missing data, encoding categorical variables, and tuning Logistic Regression and Random Forest models for optimal accuracy.

---

## 📂 Repository Contents

- `credit_card_approval.ipynb`  
  Jupyter notebook containing the full data pipeline: ingestion, cleaning, feature engineering, model training, and evaluation.

- `requirements.txt`  
  List of Python dependencies needed to run the notebook.

---

## 🖇 Data Description

The dataset (`cc_approvals.data`) contains anonymized credit card application records with both numerical and categorical attributes.  
Key fields include:  
- Applicant income, debt ratios, credit history indicators  
- Employment status, education level, and other demographic features  
- Approval decision (`approved` vs. `denied`)

---

## 🚀 Approach

1. **Data Ingestion & Cleaning**  
   - Loaded raw CSV, replaced “?” placeholders with NaN  
   - Applied median imputation for numeric columns and mode imputation for categoricals  

2. **Feature Engineering**  
   - Converted categorical fields (e.g., employment status, education) using one-hot encoding  
   - Scaled numeric features with `StandardScaler`  

3. **Model Training & Tuning**  
   - Split data into 70/30 train/test sets  
   - Trained a baseline Logistic Regression and a Random Forest classifier  
   - Performed hyperparameter tuning via `GridSearchCV`  

4. **Evaluation**  
   - Measured performance using accuracy, precision, recall, and ROC-AUC  
   - Analyzed the confusion matrix for false positive/negative trade-offs  

---

## 📈 Results & Takeaways

- **Best Model:** Random Forest achieved **85% accuracy** and **0.88 ROC-AUC** on the test set.  
- **Top Features:** Credit history length, applicant’s debt-to-income ratio, and employment duration.  
- **Business Impact:** A reliable approval predictor can reduce manual review time and improve risk management.

---

## ⚙️ Setup & Usage

1. Clone this repository:  
   ```bash
   git clone https://github.com/Zoey0227-code/credit-card-approval-predictor.git
   cd credit-card-approval-predictor
