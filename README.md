🔐💡 Fraud Detection and Subscription Pricing Optimization
This repository showcases two comprehensive data science projects focused on solving high-impact business problems through machine learning and statistical modeling: a Payment Fraud Detection & Risk Scoring System and an Optimized Subscription Pricing Strategy.

📁 Projects Breakdown
🕵️‍♂️ 1. Payment Fraud Detection & Risk Scoring System
📌 Objective
Detect fraudulent transactions in a financial dataset and assign a risk score to each transaction based on the likelihood of fraud.

📊 Dataset
Size: ~6.3 million transactions

Features: Transaction type, amount, origin and destination balances, fraud indicators

🛠 Methodology
Data Exploration: Analyzed transaction types, amounts, balance patterns, and target class distribution (severely imbalanced).

Feature Engineering:

Created derived features such as balance deltas, zero-balance flags, and transaction direction.

Dropped identifiers (nameOrig, nameDest) to prevent data leakage.

Handling Imbalance: Applied undersampling of the majority class (isFraud=0) to address extreme class imbalance.

Modeling:

Trained classification models including Random Forest and XGBoost.

Evaluated using Precision, Recall, F1-score, and ROC AUC due to class imbalance.

📈 Results
Best Model: XGBoost achieved the highest F1-score (~0.89) on the test set.

Feature Importance: Top indicators included balance discrepancies and zero old/new balances at source or destination.

Risk Scoring: Transactions were scored using model probabilities to create a custom fraud risk index.

💸 2. Optimizing Subscription Pricing
📌 Objective
Identify optimal pricing tiers for a digital subscription product to balance customer retention and revenue maximization.

📊 Dataset
Simulated user subscription dataset with features like plan type, duration, price paid, churn status, and user engagement.

🛠 Methodology
Exploratory Data Analysis:

Analyzed churn rates across pricing tiers.

Visualized customer lifetime value (CLV) and revenue contribution by price point.

Price Elasticity Modeling:

Used regression-based elasticity curves to model how demand responds to price changes.

Simulated revenue for various price points using elasticity assumptions.

Scenario Simulations:

Evaluated pricing strategies like tier bundling, discount offers, and freemium trials.

Compared churn-adjusted revenue projections for each scenario.

📈 Results
Recommended an optimal pricing range where revenue and retention were best balanced.

Demonstrated that increasing prices slightly in the middle tier improved profitability with minimal churn impact.

⚙️ Tech Stack
Languages: Python

Libraries: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn

Tools: Jupyter Notebooks

📌 How to Use
Clone the repo:

bash
Copy
Edit
git clone https://github.com/yourusername/fraud-pricing-projects.git
Open notebooks using Jupyter or VS Code

Install requirements:

bash
Copy
Edit
pip install -r requirements.txt
