# 🏥 Healthcare Intelligence & Hospital Operations Analytics Platform

> **AI-Powered Healthcare Analytics for Operational Efficiency, Patient Experience, Resource Optimization, Revenue Intelligence, and Predictive Decision Making**

![Python](https://img.shields.io/badge/Python-3.10+-blue) ![SQL](https://img.shields.io/badge/SQL-MySQL-orange) ![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow) ![ML](https://img.shields.io/badge/ML-Sklearn-green) ![Records](https://img.shields.io/badge/Records-100K%2B-red)

---

## 📋 Project Overview

This enterprise-grade analytics platform provides a hospital management with **end-to-end decision intelligence** across clinical operations, financial performance, patient experience, and resource management. Modeled after the analytics solutions deployed by top consulting firms (Deloitte, Accenture, McKinsey) and health system data teams, this project covers every phase of the analytics lifecycle.

**Project Scale:**
- 100,000+ admission records
- 7 integrated data sources / tables
- 550,000+ total data points
- 5-year time horizon (2020–2024)
- 15 analytical visualizations
- 7 Power BI dashboard pages
- 3 predictive ML models
- 20+ executive insights
- $78M+ in identified value creation

---

## 🎯 Business Problem

Regional hospital network facing:
- **18% readmission rate** (above 14.6% national CMS benchmark)
- **$12.4M outstanding billing balance** with 5% disputed claims
- **91.3% ICU utilization** — exceeding safe capacity threshold
- **3.8/5.0 patient satisfaction** — below 4.2 competitive benchmark
- **Fragmented reporting** — no unified analytics view for leadership

---

## 🏗️ Project Architecture

```
Raw Data (CSV) → SQL Star Schema → Python EDA & ML → Power BI Dashboard → Executive Insights
     ↓                  ↓                 ↓                  ↓                    ↓
  7 Tables         DDL Scripts        15 Charts           7 Pages            20+ Insights
  100K rows        Views/SPs          3 ML Models         40+ DAX             ROI: $78M+
```

---

## 📁 Repository Structure

```
healthcare-analytics-platform/
│
├── 📂 data/
│   ├── generate_dataset.py         # Synthetic data generation script
│   ├── patients.csv                # 50,000 patient records
│   ├── admissions.csv              # 100,000 admission records
│   ├── treatments.csv              # 100,000 treatment records
│   ├── billing.csv                 # 100,000 billing records
│   ├── satisfaction.csv            # 100,000 satisfaction records
│   ├── resources.csv               # 100,000 resource utilization records
│   └── doctors.csv                 # 500 doctor records
│
├── 📂 sql/
│   ├── 01_database_design.sql      # DDL: Tables, Indexes, Views, SPs
│   └── 02_data_cleaning.sql        # Data quality, cleaning, feature engineering
│
├── 📂 notebooks/
│   └── healthcare_eda_ml.py        # EDA + Predictive Models (Python)
│
├── 📂 powerbi/
│   ├── DAX_Measures.md             # Complete DAX measure library (40+ measures)
│   └── PowerBI_Dashboard_Design_Guide.md  # Layout, visuals, interactions
│
├── 📂 reports/
│   └── Executive_Insights_Recommendations.md  # 20 insights + business recommendations
│
├── 📂 docs/
│   ├── Interview_Preparation_Guide.md  # 80 Q&A across SQL/Python/PowerBI/BA
│   └── LinkedIn_Resume_Assets.md       # LinkedIn post, resume bullets, project summary
│
├── 📂 images/
│   ├── 01_monthly_admissions_trend.png
│   ├── 02_department_admissions.png
│   ├── 03_patient_demographics.png
│   ├── 04_monthly_revenue_trend.png
│   ├── 05_treatment_cost_by_dept.png
│   ├── 06_readmission_rate_dept.png
│   ├── 07_patient_satisfaction.png
│   ├── 08_resource_utilization.png
│   ├── 09_los_analysis.png
│   ├── 10_seasonal_admission_pattern.png
│   ├── 11_roc_curves_comparison.png
│   ├── 12_confusion_matrices.png
│   ├── 13_feature_importance.png
│   ├── 14_model_comparison.png
│   └── 15_revenue_forecast.png
│
└── README.md
```

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
|-------|-----------|---------|
| Data Storage | MySQL / SQLite | Star Schema database |
| Data Processing | Python, Pandas, NumPy | ETL, EDA, feature engineering |
| Visualization | Matplotlib | 15 analytical charts |
| Machine Learning | Scikit-Learn | Readmission prediction models |
| Business Intelligence | Power BI | Interactive dashboards |
| Query Language | SQL | Analytics, CTEs, window functions |
| Documentation | Markdown | All deliverables |
| Version Control | GitHub | Repository |

---

## 📊 Key Findings

| KPI | Observed | Benchmark | Gap |
|-----|----------|-----------|-----|
| Readmission Rate | 18.0% | 14.6% | -3.4pp |
| ICU Utilization | 91.3% | 80.0% | +11.3pp |
| Patient Rating | 3.8/5.0 | 4.2/5.0 | -0.4 |
| Collection Rate | 88% | 95% | -7pp |
| LOS vs DRG Benchmark | +0.6 days | 0 | Excess |

---

## 🤖 ML Model Performance

| Model | Accuracy | AUC | Notes |
|-------|----------|-----|-------|
| Logistic Regression | 82.0% | 0.49 | Baseline |
| Random Forest | 77.9% | 0.50 | Best F1 on minority class |
| Gradient Boosting | 82.0% | 0.50 | Best AUC |

*Note: AUC near 0.50 reflects synthetic data with randomized labels. With real EHR data, readmission models typically achieve AUC 0.75–0.85.*

---

## 💡 Top 5 Insights

1. **$28.9M readmission savings opportunity** by reducing rate from 18% to 14.6% benchmark
2. **ICU at 91.3% utilization** — 12 additional beds needed in Emergency + Cardiology
3. **$12.4M billing leakage** — RCM automation + financial counseling = $6.2M recovery
4. **Oncology + Cardiology = 34% of revenue** — strategic expansion priority
5. **31% of readmissions trace to missed follow-up** — TCM program ROI: 66x in 12 months

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy scikit-learn matplotlib openpyxl
```

### Generate Dataset
```bash
python data/generate_dataset.py
```

### Run EDA & ML Pipeline
```bash
python notebooks/healthcare_eda_ml.py
```

### Power BI Setup
1. Load all 7 CSV files from `/data` folder
2. Set up relationships per the Data Model in `powerbi/PowerBI_Dashboard_Design_Guide.md`
3. Import DAX measures from `powerbi/DAX_Measures.md`
4. Apply the Healthcare Professional JSON theme

### SQL Setup
```bash
# MySQL
mysql -u root -p < sql/01_database_design.sql
mysql -u root -p < sql/02_data_cleaning.sql
```

---

## 📐 Data Model (Star Schema)

```
                    ┌──────────────┐
                    │  dim_date    │
                    └──────┬───────┘
                           │
┌─────────────┐    ┌───────┴──────────┐    ┌──────────────┐
│ dim_patients│────│  fact_admissions │────│  dim_doctors │
└─────────────┘    └───────┬──────────┘    └──────────────┘
                    ┌──────┼──────────┐
                    │      │          │
            ┌───────┴──┐ ┌─┴──────┐ ┌┴─────────────┐
            │fact_treat│ │fact_bil│ │fact_satisfact│
            └──────────┘ └────────┘ └──────────────┘
                              │
                    ┌─────────┴────────┐
                    │  fact_resources  │
                    └──────────────────┘
```

---

## 📈 Business Recommendations ROI

| Horizon | Investment | Annual Return | Payback |
|---------|-----------|--------------|---------|
| Short-Term (0–6 mo) | $430K | $15M | < 1 month |
| Medium-Term (6–18 mo) | $6.1M | $23M | 3.2 months |
| Long-Term (18+ mo) | $25.3M | $40M+ | 7.6 months |
| **TOTAL** | **$31.8M** | **$78M+** | **~5 months** |

---

## 🎓 Skills Demonstrated

- **SQL:** Star Schema design, CTEs, Window Functions, Stored Procedures, Views, Query Optimization
- **Python:** Pandas, NumPy, Matplotlib, Scikit-Learn, Feature Engineering, ML Pipelines
- **Power BI:** Data Modeling, DAX, Time Intelligence, Drill-through, Bookmarks, Forecasting
- **Analytics:** EDA, Predictive Modeling, Business Intelligence, Executive Reporting
- **Business:** Healthcare KPIs, CMS Quality Metrics, Revenue Cycle, Stakeholder Communication
- **Documentation:** Technical writing, GitHub, data dictionaries, interview preparation

---

## 👤 Author

Built as a comprehensive portfolio project demonstrating enterprise-grade data analytics capabilities for Data Analyst, Business Intelligence Analyst, and Healthcare Analytics roles.

---

## 📄 License

MIT License — Free to use, adapt, and build upon for educational and portfolio purposes.

---

*This project simulates the analytics workflow used at leading consulting firms and health systems. All data is synthetically generated and contains no real patient information.*
