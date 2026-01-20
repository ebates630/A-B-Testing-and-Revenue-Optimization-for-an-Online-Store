# A/B Testing and Revenue Optimization for an Online Store

## Business Context

This project simulates a real-world analytics engagement at a large e-commerce company. The marketing and product teams generated multiple hypotheses aimed at improving revenue, user engagement, and purchasing behavior. My role was to prioritize these hypotheses, evaluate an A/B test experiment, and provide a final data-driven business recommendation.

The project follows a full experimentation lifecycle: hypothesis prioritization, experiment analysis, outlier detection, statistical testing, and executive-level conclusions.

---

## Business Objectives

- Identify high-impact, feasible optimization opportunities  
- Evaluate the performance of a new website experience  
- Measure impact on conversion rate and purchasing behavior  
- Ensure analytical rigor through data cleaning and validation  
- Provide a clear business recommendation supported by statistics  

---

## Data Sources

### hypotheses_us.csv  
Marketing hypotheses and feasibility scoring:
- Hypothesis description  
- Reach (estimated audience size)  
- Impact (expected business value)  
- Confidence (likelihood of success)  
- Effort (implementation cost)

### orders_us.csv  
Transaction-level e-commerce order data:
- transactionId  
- visitorId  
- order date  
- revenue per order  
- A/B test group

### visits_us.csv  
Daily website traffic metrics:
- date  
- A/B test group  
- total visits

---

## Phase 1: Hypothesis Prioritization

To determine which initiatives should be tested first, I applied two widely used product prioritization frameworks:

### ICE Framework  
ICE = (Impact × Confidence) / Effort  

This framework identifies ideas with strong potential impact and feasibility.

### RICE Framework  
RICE = (Reach × Impact × Confidence) / Effort  

This model was selected as the primary decision tool because it incorporates projected audience size, aligning prioritization with business scale.

### Key Insight  
The inclusion of Reach significantly altered prioritization rankings. Several hypotheses that ranked highly under ICE were deprioritized under RICE due to limited exposure, while broader-impact initiatives emerged as higher-value opportunities.

---

## Phase 2: A/B Test Design

Users were randomly assigned to one of two groups:

- Group A: Control experience (existing website)  
- Group B: Test experience (new optimization)

The experiment tracked purchasing behavior and revenue performance over time.

---

## Phase 3: Exploratory Performance Analysis

### Cumulative Revenue  
Group B generated consistently higher cumulative revenue, indicating improved monetization performance.

### Cumulative Average Order Size  
Average purchase value remained comparable across groups, with intermittent volatility driven by large purchases.

### Relative Difference in Average Order Size  
Differences fluctuated near zero, suggesting no stable advantage in order value.

### Daily Conversion Rate  
Group B demonstrated higher daily conversion rates, indicating increased likelihood of purchase.

### Behavioral Outliers  
Order frequency and purchase price distributions revealed a small number of abnormal users and transactions with disproportionate influence.

---

## Phase 4: Outlier Treatment

To prevent distortion of experimental results, outliers were identified using percentile-based thresholds and removed from the filtered dataset. This allowed for a more accurate assessment of typical customer behavior.

---

## Phase 5: Statistical Validation

Formal hypothesis testing was conducted on both raw and filtered datasets.

### Tests Performed

- Conversion rate comparison (Z-test)  
- Average order value comparison (Mann–Whitney U test)  

Each test was executed on:
- Raw data  
- Filtered data  

---

## Results Summary

- Conversion rate improvement for Group B was statistically significant  
- No statistically significant difference in average order value  
- Filtered results confirmed raw data findings  

---

## Final Business Recommendation

The experiment demonstrates that the test experience (Group B) produces a statistically significant lift in conversions without negatively impacting order value. Based on these results, the experiment should be concluded and the Group B experience rolled out.

This change is expected to increase revenue primarily through higher transaction volume rather than increased basket size.

---

## Analytical Skills Demonstrated

- Experiment design and evaluation  
- Product hypothesis prioritization  
- Behavioral analytics  
- Outlier detection and treatment  
- Statistical inference  
- Business-focused storytelling  
- Executive decision support  

---

## Technology Stack

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Jupyter Notebook  
- Z-test, Mann–Whitney U test  

---

## Repository Structure

data/  
notebooks/  
README.md  

---

## Outcome

This project demonstrates the end-to-end workflow of data-driven experimentation, from ideation through executive-level decision-making. The approach mirrors real-world product and marketing analytics used in revenue optimization initiatives across e-commerce organizations.

