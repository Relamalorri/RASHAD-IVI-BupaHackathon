# IVI Scoring Methodology

## Overview
The Intelligent Value Index (IVI) is a composite risk score ranging from 0 to 100 assigned to each corporate insurance contract. A higher score indicates lower risk and better portfolio value. The model was built using anonymized 3-year data provided by Bupa Arabia.

---

## Formula

IVI = 0.294 x H + 0.115 x E + 0.591 x U

---

## Dimensions

### H — Health Outcomes (29.4%)
Measures medical complexity and clinical risk at the contract level.

| Metric | Description |
|--------|-------------|
| Chronic condition burden | Proportion of members with chronic diagnoses |
| High-risk diagnosis rate | Rate of high-cost or severe diagnoses |
| Health risk escalation | Year-over-year change in health risk indicators |

### E — Experience Performance (11.5%)
Evaluates service quality and member satisfaction.

| Metric | Description |
|--------|-------------|
| Rejection rate | Rate of pre-authorization and claim rejections |
| Complaint frequency | Volume of complaints per member |
| Service quality delays | Average response and resolution time |

### U — Utilization Efficiency (59.1%)
Measures cost efficiency and consumption patterns.

| Metric | Description |
|--------|-------------|
| Cost per member | Net bill divided by number of utilizers |
| High-cost service rate | Proportion of high-cost service episodes |
| Services per episode | Average number of services per treatment episode |

---

## Dimension Weights
Weights were derived data-driven using portfolio pain-point analysis. Utilization Efficiency received the highest weight (59.1%) as it was identified as the primary driver of portfolio risk, nearly twice as impactful as Health Outcomes.

---

## Data Processing Pipeline

| Step | Description |
|------|-------------|
| 1. Sampling and Extraction | Raw SAS datasets sampled and extracted |
| 2. Cleaning and Validation | Missing values imputed using portfolio medians |
| 3. Aggregation | Member-level data aggregated to contract level |
| 4. Normalization | Z-score standardization applied across all metrics |
| 5. Scoring | Weighted composite score calculated per contract |

---

## Key Assumptions
- 12-month rolling analysis period used for all metrics
- Missing values imputed using portfolio medians
- Z-score standardization applied before weighting
- Retention probability inferred using IVI level and experience trends as a proxy for churn risk

---

## Model Limitations
- Historical bias may exist in training data
- Model requires periodic retraining as portfolio evolves
- Retention probability is a proxy, not a directly observed variable
