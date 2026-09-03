# Customer Churn Prediction

Part 2 of the **AI for Communication and Marketing** project  
BSc in Artificial Intelligence — University of Pavia, A.Y. 2025/2026.

## Objective

The goal of this project is to identify customers at risk of churn and use predictive modeling to support targeted retention strategies.

The analysis focuses not only on predictive performance, but also on the business impact of different model errors.

## Methods

- Data preprocessing and exploratory analysis
- Train/test split with stratification
- Logistic Regression
- Random Forest
- Class imbalance handling
- Feature importance analysis
- Confusion Matrix
- ROC-AUC evaluation
- Lift and risk-decile analysis

## Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

The **Random Forest** achieved the strongest overall performance:

| Metric | Score |
|---|---:|
| Accuracy | 0.928 |
| Precision | 0.745 |
| Recall | 0.873 |
| F1-score | 0.804 |
| ROC-AUC | 0.976 |

Recall was prioritized because missing an actual churner was considered more costly than targeting a retained customer.

## Key Findings

The analysis identified several important churn drivers, including:

- Customer tenure
- Complaints
- Cashback amount
- Time since last order

Customers in the first months of their lifecycle showed particularly high churn risk.

Ranking customers by predicted churn probability also showed that targeting the **top 20% highest-risk customers captures approximately 74% of churners**, allowing retention actions to be focused on a smaller portion of the customer base.

## Business Application

The model results were translated into a two-wave retention strategy:

- Early-lifecycle onboarding for recently acquired high-risk customers
- Complaint-recovery actions for dissatisfied customers

## Files

- `churn_prediction.ipynb` — full analysis and modeling
- `churn_prediction_presentation.pdf` — summary of results and retention strategy

## Author

**Marta Paniconi**
