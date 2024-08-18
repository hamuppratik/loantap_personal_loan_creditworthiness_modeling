LoanTap Underwriting Model:
- LoanTap is an online platform that offers flexible loan products to salaried professionals.

In this project, LoanTap aimed to develop an underwriting model to assess the creditworthiness of individuals seeking personal loans. The model's objective was to evaluate attributes to determine loan approval and recommend appropriate repayment terms, aligning with LoanTap's commitment to flexible, consumer-friendly loans for salaried professionals and businessmen.

Problem Definition:

Objective: Build a model to assess creditworthiness for personal loan applicants and recommend suitable repayment terms.
Scope: Evaluate attributes to determine loan approval and ensure alignment with LoanTap's flexible loan offerings.
Insights from Exploratory Data Analysis:

Impact of Categorical Attributes:

Loan Term: Longer loan terms (60-month) have a higher default rate.
Grade/Sub-Grade: Higher grades have more defaults, indicating grade/sub-grade is a significant factor in loan status.
Application Type: Direct pay applications have a higher default rate compared to individual or joint applications.
Loan Purpose: Loans for small business purposes show the highest default rates.
Irrelevant Attributes: Initial list status and emp_title/title have no significant impact on loan status and can be removed.
Impact of Numerical Attributes:

Defaulter Characteristics: Defaulters tend to have higher mean values for loan amount, interest rate, debt-to-income ratio (dti), number of open accounts, and revolving credit utilization. They also have a lower mean annual income.

Model Performance:

Logistic Regression Model:
Accuracy: 80%
Precision (Negative Class): 94%
Recall (Negative Class): 82%
F1 Score (Negative Class): 87%
Precision (Positive Class): 52%
Recall (Positive Class): 82%
F1 Score (Positive Class): 87%
ROC AUC Score: 0.90, indicating strong differentiation between classes.
Precision-Recall AUC Score: 0.78, which could be improved through hyperparameter tuning or using more complex models.

Recommendations:

Optimize Risk and Opportunity Balance: Aim to maximize the F1 score and the area under the Precision-Recall Curve to balance the risk of non-performing assets (NPAs) and the opportunity to extend loans to creditworthy customers.
Consider More Complex Models: Explore advanced classifiers like Random Forest, which can handle non-linear decision boundaries and potentially provide better results than logistic regression.
