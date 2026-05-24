# RASHAD — Risk Intelligence
### Intelligent Value Index (IVI) Analytics Engine
**Futurethon x Bupa Arabia HealthTech Hackathon — 3rd Place**

---

## What is RASHAD?
RASHAD (Risk Assessment & Strategic Health Analytics Dashboard) is a data-driven risk scoring framework built for Bupa Arabia's corporate insurance portfolio. It assigns every corporate client an Intelligent Value Index (IVI) Score from 0–100, enabling proactive risk management and retention strategies.

---

## The IVI Formula

IVI = 0.294 x H + 0.115 x E + 0.591 x U

| Dimension | Weight | Description |
|-----------|--------|-------------|
| H — Health Outcomes | 29.4% | Chronic conditions, high-risk diagnoses, medical complexity |
| E — Experience Performance | 11.5% | Rejection rates, complaint frequency, service delays |
| U — Utilization Efficiency | 59.1% | Cost per member, high-cost service rate, services per episode |

---

## Key Results

| Metric | Value |
|--------|-------|
| Total Contracts Scored | 31,617 |
| High-Risk Contracts | 10,225 (32.3%) |
| Low-Risk Contracts | 21,392 (67.7%) |
| Key Finding | Bimodal distribution — contracts polarize between scores 5–50 and 75–95 |

---

## Repo Structure

| Folder / File | Description |
|---------------|-------------|
| README.md | Project overview and documentation |
| docs/rashad-pitch.pdf | Project pitch deck and executive summary presented at Futurethon 2025 |
| data/Data_dictionary.xlsx | Column definitions for all datasets provided by Bupa Arabia |
| data/Provider_Info.xlsx | Hospital and clinic reference information |
| data/README.md | Notes on raw datasets not included in repo |
| model/IVI_methodology.md | IVI scoring logic, assumptions, and full methodology documentation |
| notebooks/README.md | Code files to be added |

---

## Live Dashboard
[rashad.manus.space](https://rashad.manus.space)

---

## Built With

| Tool | Purpose |
|------|---------|
| Python | Data processing and IVI scoring model |
| Power BI | Data exploration and visualization |
| Manus AI | Dashboard development and deployment |
| Excel | Initial data exploration and validation |

---

## Disclaimer
All data used is anonymized sample data provided by Bupa Arabia for educational purposes only and does not represent real individuals or records.
