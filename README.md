# Taxi Fare EDA & Hypothesis Testing 🚕📊

## Overview
This project performs **Exploratory Data Analysis (EDA)** and **statistical hypothesis testing** on New York City taxi trip data to examine how **payment method (Card vs Cash)** influences **fare amount and trip characteristics**.  
The goal is to derive **data-driven insights** that can help improve **revenue optimization strategies** for taxi drivers and platforms.

---

## Business Context
Taxi and ride-hailing platforms aim to maximize driver earnings while maintaining a smooth customer experience.  
Understanding whether **payment behavior affects fare value** can support better payment incentives and operational decisions.

---

## Objectives
- Explore fare and trip patterns across different payment methods
- Compare **average fare amounts** for card and cash payments
- Apply **statistical hypothesis testing** to validate observed differences
- Draw actionable insights based on analytical evidence

---

## Research Question
> Does the average taxi fare differ significantly between **card payments** and **cash payments**?

---

## Dataset
- **Source**: NYC Yellow Taxi Trip Data
- **File Used**: `yellow_tripdata_2020-01.csv`
- **Initial Records**: ~1 million trips
- **Final Dataset**: **1,048,575 rows × 5 columns** (after cleaning)

### Key Features
- `fare_amount`
- `payment_type`
- `trip_distance`
- `passenger_count`
- `trip_duration`

---

## Data Cleaning & Preparation
- Removed missing and invalid records
- Selected relevant analytical columns
- Filtered payment types to **Card** and **Cash**
- Checked and handled duplicates
- Ensured correct data types for analysis

---

## Exploratory Data Analysis (EDA)
The following analyses were conducted:
- Fare amount distribution by payment type
- Trip distance comparison across payment methods
- Passenger count analysis
- Payment method frequency analysis
- Summary statistics (mean, standard deviation)
- Visualizations using histograms, bar charts, and pie charts

---

## Key Insights
- **Card payments are more frequent** than cash payments
- **Higher average fares** are associated with card transactions
- Longer trips tend to be paid by card
- Single-passenger trips dominate across both payment types
- Statistical evidence supports promoting card-based payments for higher revenue efficiency
  
---

## Hypothesis Testing
### Hypotheses
- **Null Hypothesis (H₀)**: There is no difference in average fare amount between card and cash payments
- **Alternative Hypothesis (H₁)**: There is a significant difference in average fare amount between card and cash payments

### Statistical Method
- **Welch’s Independent t-test**
- Suitable for samples with unequal variances

### Results
- **t-statistic**: 54.58
- **p-value**: < 0.05

**Decision**: Reject the null hypothesis  
There is a **statistically significant difference** in average fares between payment methods.

---

## Conclusion
- Payment method has a measurable impact on fare amount
- **Card payments generate higher average fares**
- Encouraging digital payments could improve driver revenue
- Findings support **data-backed decision-making** for taxi platforms

---

## Tools & Technologies

| Language / Platform | Libraries   |
|---------------------|-------------|
| Python              | Pandas      |
| Jupyter Notebook    | NumPy       |
|                     | Matplotlib  |
|                     | Seaborn     |
|                     | SciPy       |
|                     | StatsModels |

---

## Project Structure
```
📦 taxi-fare-eda-hypothesis-testing
│
├── 📂 data
│   └──  yellow_tripdata_2020-01.csv
│
├── Taxi_Fare_Analysis_and_Hypothesis_Testing.ipynb
├── README.md
├── .gitignore
└── LICENSE
```
---

## License

This project is licensed under the **MIT License**.

---
