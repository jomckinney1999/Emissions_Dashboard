# 🌍 US County-Level Emissions Dashboard (2023)

![Databricks](https://img.shields.io/badge/Built%20with-Databricks-FF3621?style=flat&logo=databricks&logoColor=white)
![Data](https://img.shields.io/badge/Data-2023%20Emissions-00B4D8?style=flat)
![Scope](https://img.shields.io/badge/Scope-US%20County--Level-2ECC71?style=flat)

An interactive data visualization dashboard built on **Databricks** that explores 2023 county-level greenhouse gas emissions across the United States. The dashboard surfaces geographic, demographic, and comparative emissions insights through a suite of coordinated visualizations.

---

## 📊 Dashboard Overview

The dashboard is composed of four key panels:

### 1. 🗺️ Geographic Emissions Map
A Mapbox-powered dot-density map plotting emissions across all US counties. Each point represents a county-level data record, allowing users to instantly spot regional emissions hotspots and density clusters from coast to coast.

### 2. 📉 Emissions Per Person vs. Population (Scatter Plot)
A scatter plot correlating **per-capita emissions** (x-axis) with **county population** (y-axis). This chart reveals an important story: high-population metros don't necessarily have the worst per-capita emissions — smaller, more industrial counties often do.

### 3. 🍩 Top 10 States — Emissions Percentage (Donut Chart)
A donut chart breaking down the share of total US emissions attributed to the top 10 emitting states. Key findings:
- **TX** leads at **20.63%**
- **FL** follows at **16.47%**
- **OH** at **9.71%**, **IL** at **9.13%**
- Together, the top 10 states account for **51% of all US emissions**

### 4. 📊 Total Emissions by County — mTon CO₂e (Bar Chart)
A ranked horizontal bar chart of the top 10 highest-emitting counties by total emissions in metric tons of CO₂ equivalent:

| Rank | County | Total Emissions |
|------|--------|----------------|
| 1 | Maricopa County, AZ | 9.81M mTon |
| 2 | Harris County, TX | 9.68M mTon |
| 3 | Cook County, IL | 8.11M mTon |
| 4 | Miami-Dade County, FL | 5.62M mTon |
| 5 | Dallas County, TX | 5.43M mTon |
| 6 | Los Angeles County, CA | 5.00M mTon |
| 7 | Tarrant County, TX | 4.48M mTon |
| 8 | Broward County, FL | 4.41M mTon |
| 9 | Clark County, NV | 4.24M mTon |
| 10 | Bexar County, TX | 3.82M mTon |

---

## 🛠️ Tech Stack

| Tool | Role |
|------|------|
| **Databricks** | Data processing, compute, and dashboard hosting |
| **Mapbox** | Interactive geographic map rendering |
| **SQL / PySpark** | Data transformation and aggregation |
| **Databricks Lakestore** | Data storage and querying |

---

## 🔍 Key Insights

- **Texas dominates** US emissions both at the state level (20.63%) and county level, with 3 of the top 10 emitting counties.
- **Maricopa County, AZ** (Phoenix metro) is the single highest-emitting county despite not belonging to a traditionally "industrial" state.
- **Per-capita emissions are inversely correlated with population density** — rural and industrial counties tend to emit significantly more per person than large urban metros.
- The **top 10 states collectively account for ~51%** of all US greenhouse gas emissions.

---

## 📁 Project Structure

```
emissions-dashboard/
│
├── notebooks/
│   ├── 01_data_ingestion.py
│   ├── 02_data_cleaning.py
│   └── 03_aggregations.py
│
├── dashboard/
│   └── emissions_dashboard_view.json
│
└── README.md
```

---

## 🚀 Getting Started

1. Clone this repository
2. Import the notebooks into your Databricks workspace
3. Run notebooks in sequence (`01` → `02` → `03`)
4. Open the Databricks Dashboard view and attach to your cluster

---

## 📌 Data Source

2023 US County-Level Greenhouse Gas Emissions dataset. Units are reported in **metric tons of CO₂ equivalent (mTon CO₂e)**.

---

## 📬 Contact

Feel free to open an issue or reach out if you have questions about the methodology or data sources.
