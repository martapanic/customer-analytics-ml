# Customer Lifetime Value Forecasting

Part 3 of the **AI for Communication and Marketing** project  
BSc in Artificial Intelligence — University of Pavia, A.Y. 2025/2026.

## Objective

The goal of this project is to estimate future customer value and compare probabilistic customer-lifetime models with machine learning approaches for short-term revenue forecasting.

The analysis also explores how Customer Lifetime Value can support customer targeting and marketing decisions.

## Methods

- Transaction-level data preparation
- RFM feature engineering
- Calibration and holdout periods
- BG/NBD modeling
- Gamma-Gamma monetary model
- Customer Lifetime Value estimation
- Random Forest regression
- Revenue forecasting
- Customer segmentation based on CLTV and probability of being alive

## Models

Two different modeling approaches were compared:

### Probabilistic BTYD approach

- BG/NBD for purchase frequency and customer activity
- Gamma-Gamma for expected monetary value

### Machine Learning approach

- Random Forest Regression for short-term revenue prediction

## Model Comparison

| Model | MAE | RMSE |
|---|---:|---:|
| BG/NBD + Gamma-Gamma | 1.90 | 15.22 |
| Random Forest | 1.65 | 14.77 |

Random Forest provided lower prediction error for short-term forecasting, while the probabilistic model offered interpretable customer-level signals such as expected CLTV and probability of being alive.

## Customer Segmentation

The probabilistic model was also used to define actionable customer groups:

- **Retain** — High CLTV, high probability of being alive
- **Win-Back** — High CLTV, low probability of being alive
- **Nurture** — Low CLTV, high probability of being alive
- **Monitor** — Low CLTV, low probability of being alive

These segments were translated into differentiated retention and re-engagement strategies.

## Files

- `cltv_forecasting.ipynb` — full analysis and modeling
- `cltv_forecasting_presentation.pdf` — summary of results and business recommendations

## Author

**Marta Paniconi**
