# Customer Analytics & Marketing Intelligence

A collection of three applied customer analytics projects developed for the
**AI for Communication and Marketing** course during my BSc in Artificial Intelligence
at the University of Pavia.

The projects explore different stages of the customer analytics lifecycle:
**segmentation, churn prediction, and Customer Lifetime Value forecasting**.

Each analysis combines data-driven modeling with the translation of results
into actionable business and marketing strategies.

---

## Projects

### 1. Customer Segmentation & Communication Strategy

Customer segmentation using both **RFM analysis** and **K-Means clustering**
to identify high-value customer groups and design differentiated communication strategies.

#### Methods
- Data cleaning and exploratory data analysis
- RFM customer segmentation
- Feature scaling
- K-Means clustering
- Elbow method and Silhouette Score
- PCA
- Cluster profiling
- Marketing strategy development

#### Key Findings

RFM analysis identified a strong concentration of value among top customer segments,
while K-Means provided complementary behavioral personas.

The **Premium Lifestyle** cluster, representing 23.8% of customers,
generated 51.6% of total revenue.

The results were translated into differentiated communication strategies,
including premium retention, reactivation, conversion and low-cost nurturing campaigns.

---

### 2. Customer Churn Prediction

Supervised machine learning project designed to identify customers at risk of churn
and prioritize retention efforts.

#### Models
- Logistic Regression
- Random Forest

#### Evaluation
Models were compared using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- Lift analysis

#### Results

The Random Forest model achieved:

| Metric | Score |
|---|---:|
| Accuracy | 0.928 |
| Precision | 0.745 |
| Recall | **0.873** |
| F1-score | 0.804 |
| ROC-AUC | **0.976** |

Recall was prioritized because failing to identify an actual churner was considered
more costly than targeting an additional retained customer.

Ranking customers by predicted churn probability showed that the **top 20% risk segment
captures approximately 74% of churners**, enabling more efficient retention campaigns.

---

### 3. Customer Lifetime Value Forecasting

Customer value modeling and revenue forecasting using both
**probabilistic BTYD models** and machine learning regression.

#### Models
- BG/NBD
- Gamma-Gamma
- Random Forest Regression

#### Analysis
- Transaction-level data preparation
- RFM feature engineering
- Calibration / holdout evaluation
- Customer Lifetime Value estimation
- Revenue forecasting
- Customer segmentation using expected CLTV and probability of being alive

#### Results

For short-term revenue prediction, Random Forest achieved lower prediction error
than the probabilistic BTYD approach.

| Model | MAE | RMSE |
|---|---:|---:|
| BG/NBD + Gamma-Gamma | 1.90 | 15.22 |
| Random Forest | **1.65** | **14.77** |

The probabilistic model remains useful for interpreting customer behavior through
metrics such as expected CLTV and `p(alive)`, while the machine learning model
provided stronger short-term forecasting performance.

---

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Lifetimes
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Repository Structure

```text
customer-analytics-ml/
│
├── 01-customer-segmentation/
│   ├── customer_segmentation.ipynb
│   └── presentation.pdf
│
├── 02-churn-prediction/
│   ├── churn_prediction.ipynb
│   └── presentation.pdf
│
├── 03-customer-lifetime-value/
│   ├── cltv_forecasting.ipynb
│   └── presentation.pdf
│
├── requirements.txt
└── README.md
