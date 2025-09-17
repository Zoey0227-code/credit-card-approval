Credit Card Approval Predictor

A machine learning project that predicts credit card application approvals using demographic and financial data. Demonstrates expertise in data cleaning, feature engineering, model training, and hyperparameter tuning to support better credit risk decisions.

🔑 Key Features

Data preprocessing

Replaced missing values with median/mode imputation.

Encoded categorical variables with one-hot encoding.

Scaled numeric features using StandardScaler.

Modeling & optimization

Trained baseline Logistic Regression and Random Forest classifiers.

Applied GridSearchCV to tune hyperparameters for improved performance.

Evaluation & insights

Assessed models with accuracy, precision, recall, and ROC-AUC.

Random Forest achieved 85% accuracy and 0.88 ROC-AUC.

Key drivers of approval included credit history length, debt-to-income ratio, and employment duration.

🛠️ Tech Stack

Python (pandas, scikit-learn, NumPy, Matplotlib, Seaborn)

Jupyter Notebook for experimentation and documentation

📂 Project Structure
credit_card_approval.ipynb   # End-to-end data pipeline and modeling
requirements.txt             # Dependencies for reproducibility
cc_approvals.data            # Anonymized dataset (input)

🚀 Outcome

✔ Built a reliable credit approval predictor that reduces manual reviews
✔ Showcased ability to handle mixed data types and missing values
✔ Demonstrated translating ML models into business impact (risk reduction, efficiency)
