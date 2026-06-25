# Kartikeya Vemula

### Data Analyst · Product Analytics · Business Intelligence · Analytics Engineering
🏅 **Certified:** Microsoft Power BI Data Analyst Associate (PL-300) · dbt Fundamentals (dbt Labs)

<p align="center">
  <a href="mailto:vnskartikeya@gmail.com"><img src="https://img.shields.io/badge/Email-vnskartikeya%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://linkedin.com/in/kartikeya-vemula"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://your-portfolio-link.com"><img src="https://img.shields.io/badge/Portfolio-View-222222?style=for-the-badge&logo=github&logoColor=white"/></a>
  <a href="https://github.com/Kartz82"><img src="https://img.shields.io/badge/GitHub-Kartz82-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
  <a href="https://drive.google.com/file/d/1RauajCNuEzpdk_8BNsy8GinxvrOfHxfQ/view?usp=sharing"><img src="https://img.shields.io/badge/Resume-View-4CAF50?style=for-the-badge&logo=googledrive&logoColor=white"/></a>
</p>

> 🟢 **Open to:** Data Analyst · Product Analyst · BI Analyst · Analytics Engineer · Risk Analytics roles
---

## About

Data Analyst focused on **product analytics, customer intelligence, business intelligence, KPI diagnostics, experimentation, and risk analytics**. I build end-to-end analytics systems — from data pipelines and warehouses to executive dashboards and statistical models — and translate outputs into stakeholder-ready decisions.

**Core stack:** `SQL` · `Python` · `PostgreSQL` · `BigQuery` · `Power BI` · `Plotly` · `Docker` · `XGBoost`

---

## Analytics Domains

| Domain | What I Build |
|---|---|
| **Customer & Product Analytics** | RFM segmentation, cohort analysis, CLV, retention/churn modeling, funnel analysis |
| **Business Intelligence** | Star-schema warehouses, executive dashboards, KPI monitoring, geographic BI |
| **Experimentation** | A/B test frameworks, lift estimation, statistical significance, variant reporting |
| **Risk Analytics** | Tail-risk modeling, Extreme Value Theory, anomaly detection, threshold diagnostics |
| **Analytics Engineering** | ETL pipelines, dimensional modeling, data quality & QA, idempotent upserts |
| **Forecasting** | Time series modeling, multi-asset forecasting, rolling diagnostics |

---

## Featured Analytics Systems

---

### 📊 [Customer Segmentation & Retention Intelligence Platform](https://github.com/Kartz82)

**Problem:** A retail business needed to identify which customers drove revenue, which were at risk of lapsing, and where lifecycle marketing investment would generate the highest ROI.

Built an RFM segmentation engine on 1M+ transactions, classifying 5,876 customers into 8 behavioral tiers using SQL window functions. Delivered cohort retention dashboards, CLV analysis, and executive reporting to quantify revenue concentration and flag at-risk accounts.

- **Champions (22.1% of customers) drove 68.35% of total revenue**
- **£171K+ revenue identified at risk across 15 high-value inactive customers**

`Python` `SQL` `PostgreSQL` `RFM` `CLV` `Cohort Analysis` `Plotly`

---

### 🔁 [Growth Funnel Intelligence Engine](https://github.com/Kartz82)

**Problem:** A product team needed visibility into where users were dropping out of the acquisition funnel and how conversion varied across segments, channels, and time.

Built a multi-stage funnel analytics system with step-level conversion tracking, segment breakdowns, and time-windowed cohort views. Output designed for product and marketing stakeholders with drill-down capability.

`Python` `SQL` `Funnel Analysis` `Cohort Analysis` `Product Analytics` `Plotly`

---

### 🛒 [Instacart Customer & Operations Intelligence Platform](https://github.com/Kartz82)

**Problem:** A high-volume grocery dataset needed to be turned into an actionable intelligence system across customer behavior, merchandising, and reorder analytics.

Engineered a Dockerized PostgreSQL warehouse ingesting 3.4M+ orders across 206K customers and 49K SKUs. Built RFM segmentation, market basket analysis via Apriori, and a 4-tab Plotly Dash dashboard connected live to the database.

- **55,092 at-risk customers identified (26.7% of base)**
- **Apriori: 3.26 lift, 29.1% confidence on key product associations**

`Python` `PostgreSQL` `Docker` `SQL` `Apriori` `Plotly Dash` `Market Basket Analysis`

---

### 🔬 [KPI Reliability & Diagnostic Engine](https://github.com/Kartz82)

**Problem:** Analysts were spending hours manually investigating KPI drops with no systematic way to surface the root segment or attribute causing a deviation.

Built an end-to-end KPI monitoring pipeline with 0–100 data health scores, volume/null checks, rolling z-score anomaly detection, and structured JSON diagnostics. Automated root cause analysis pinpointed Mobile/APAC/Safari as the primary segment offender (−9.2% change).

`Python` `SQL` `BigQuery-Compatible Schema` `Anomaly Detection` `Rolling Z-Score` `Plotly` `YAML`

---

### 🏗️ [Customer Intelligence Data Warehouse](https://github.com/Kartz82)

**Problem:** Raw e-commerce transactions across 43 countries needed to be ingested, validated, and structured to support consistent AOV, repeat purchase, and LTV reporting.

Cleaned and modeled 1,067,371 transactions into a Dockerized PostgreSQL star-schema warehouse with fact and dimension tables. Extended the pipeline with a validated dbt transformation layer — implementing staging, intermediate, and mart models for AOV, repeat purchase rate, CLV, country revenue, and monthly sales reporting. Enforced data quality through 41 dbt tests covering uniqueness, null validation, and referential integrity across 14 successfully built models. Generated BI-ready CSV exports, dbt documentation, and DAX and Power Query workflow documentation for executive performance monitoring in Power BI.

- **14 dbt models built · 41 dbt tests passed · dbt docs generated**
- **Executive KPI marts cover AOV, Repeat Purchase Rate, CLV, Country Revenue, and Monthly Sales across 43 countries**

`Python` `PostgreSQL` `Docker` `SQL` `dbt` `ETL` `Star Schema` `Analytics Engineering` `Data Quality` `Power BI`

---

### 🌫️ [Extreme-Value AQI Risk Modeling for Baltimore Air Quality](https://github.com/Kartz82/Extreme-Value-AQI-Prediction-for-Baltimore-City)

**Problem:** Air quality data from the EPA is fragmented, inconsistent, and not structured for predictive modeling or tail-risk analysis out of the box.

Rebuilt a reproducible EPA AirData pipeline for the Baltimore-Columbia-Towson region, consolidating AQI, pollutant (CO, Ozone, NO2, PM2.5, PM10, SO2), and meteorological predictors into a 6,573-row modeling dataset (2006–2023). Benchmarked 8 regression models; tuned XGBoost was best-in-class. Applied Extreme Value Theory (Peaks-over-Threshold, GPD) to 98 threshold exceedances to quantify severe AQI tail risk.

- **Tuned XGBoost: RMSE 8.99, MAE 5.52, R² 0.852**
- **98 exceedances above AQI 150 (1.49% exceedance rate)**
- **P(AQI > 200 | AQI > 150) = 6.65% via GPD tail fit**

`Python` `EPA AirData` `XGBoost` `Extreme Value Theory` `GPD` `Risk Analytics` `Forecasting`

---

## Additional Work

| Project | Description |
|---|---|
| **A/B Experimentation Engine** | Statistical testing framework for lift estimation, significance testing, and variant reporting |
| **Multi-Asset Forecasting Pipeline** | Time series forecasting across multiple assets with rolling evaluation and performance tracking |
| **Engineering Analytics Warehouse** | GitHub REST API ETL into PostgreSQL star schema; SQL window functions for commit velocity and productivity reporting |

---

## Technical Stack

| Layer | Tools |
|---|---|
| **Languages** | Python · SQL |
| **Databases** | PostgreSQL · BigQuery |
| **Analytics & ML** | scikit-learn · XGBoost · SciPy · pandas · NumPy |
| **Visualization** | Plotly · Plotly Dash · Power BI · Looker Studio · Tableau |
| **Engineering** | Docker · dbt · Git · REST APIs · ETL Pipelines |
| **Methods** | RFM · CLV · Cohort Analysis · A/B Testing · Anomaly Detection · Extreme Value Theory · Star Schema · Dimensional Modeling |

---

## Currently

- 📍 M.S. Data Science, UMBC — GPA 3.78 (2024–2026)
- 🔬 Graduate Research Assistant — Risk Analytics (AQI modeling, EVT)
- 🎯 Actively seeking full-time roles in **Data Analytics · Product Analytics · BI · Analytics Engineering**

---

## Contact

<p align="center">
  <a href="mailto:vnskartikeya@gmail.com"><img src="https://img.shields.io/badge/Email-vnskartikeya%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://linkedin.com/in/kartikeya-vemula"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://your-portfolio-link.com"><img src="https://img.shields.io/badge/Portfolio-View-222222?style=for-the-badge&logo=github&logoColor=white"/></a>
</p>

<p align="center">📞 +1 (443) 630-1157</p>
