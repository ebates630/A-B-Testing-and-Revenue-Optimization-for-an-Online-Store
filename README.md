# A/B Testing and Revenue Optimization for an Online Store

## Business Context

An A/B test was conducted for a large online retailer to evaluate whether a new website experience improved customer purchasing behavior and revenue performance. Marketing and product teams developed several hypotheses focused on increasing conversion rates and overall revenue. I was responsible for prioritizing these hypotheses, analyzing the experiment results, and delivering a final data-driven business recommendation.

This work follows an end-to-end experimentation workflow including hypothesis prioritization, experiment analysis, outlier detection, statistical validation, and executive-level conclusions.

---

## Business Objectives

- Identify high-impact, feasible revenue opportunities  
- Evaluate the performance of a new website experience  
- Measure impact on customer conversion and purchasing behavior  
- Ensure analytical accuracy through data cleaning and validation  
- Deliver a clear, actionable business recommendation  

---

## Data Sources

hypotheses_us.csv  
Marketing hypotheses and feasibility scoring:
- Hypothesis description  
- Reach  
- Impact  
- Confidence  
- Effort  

orders_us.csv  
Transaction-level e-commerce data:
- transactionId  
- visitorId  
- order date  
- revenue  
- A/B test group  

visits_us.csv  
Daily website traffic data:
- date  
- A/B test group  
- total visits  

---

## Phase 1: Hypothesis Prioritization

To determine which initiatives should be tested first, two product prioritization frameworks were applied.

ICE = (Impact × Confidence) / Effort  
RICE = (Reach × Impact × Confidence) / Effort  

Including Reach significantly changed prioritization outcomes. Several ideas that initially appeared high-value were deprioritized due to limited exposure, while broader initiatives emerged as stronger revenue opportunities.

---

## Phase 2: Experiment Design

Users were randomly assigned into two groups:

- Group A — existing website experience  
- Group B — optimized website experience  

The experiment tracked purchasing behavior, traffic patterns, and revenue performance over time.

---

## Phase 3: Performance and Behavioral Analysis

- Group B consistently generated higher cumulative revenue.  
- Average order value remained similar between groups, with volatility caused by large purchases.  
- Relative differences in order size fluctuated near zero, showing no stable basket size advantage.  
- Group B demonstrated higher daily conversion rates.  
- A small number of users and transactions showed abnormal behavior.

---

## Phase 4: Outlier Treatment

Outliers were identified using percentile-based thresholds and removed from the filtered dataset to prevent distorted results and better represent typical customer behavior.

---

## Phase 5: Statistical Validation

Formal hypothesis testing was conducted on both raw and filtered datasets.

Tests performed:
- Conversion rate comparison (Z-test)  
- Average order value comparison (Mann-Whitney U test)  

Each test was run on raw and filtered data.

---

## Results Summary

- Group B showed a statistically significant improvement in conversion rate.  
- No statistically significant difference was observed in average order value.  
- Filtered results confirmed the raw data findings.

---

## Final Business Recommendation

The optimized website experience (Group B) produced a statistically significant lift in conversions without negatively impacting order value. Based on these results, the experiment should be concluded and the Group B experience rolled out.

Revenue growth is expected to come primarily from higher transaction volume rather than increased basket size.

---

## Analytical Skills Demonstrated

- A/B testing and experiment evaluation  
- Hypothesis prioritization  
- Data cleaning and validation  
- Customer behavior analysis  
- Outlier detection  
- Statistical testing  
- Business decision-making  

---

## Technology Stack

Python  
Pandas, NumPy  
Matplotlib, Seaborn  
Jupyter Notebook  
Z-test, Mann-Whitney U test  

---

## Repository Structure

data/  
notebooks/  
README.md  

---

## Outcome

This project demonstrates the end-to-end workflow of data-driven experimentation, from ideation through executive-level decision-making. The approach mirrors real-world product and marketing analytics used in revenue optimization initiatives across e-commerce organizations.

