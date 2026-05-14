# The Nigerian Budget Analytics Dashboard

> A 3-page Power BI dashboard built as a modeled/simulated analytics project based on Nigerian budget data, the dashboard transforms complex public finance information into an interactive and accessible analytical experience

<img width="1920" height="3411" alt="The 2026 Nigerian Budget Dashboard Suite" src="https://github.com/user-attachments/assets/c83f12da-169b-4e1a-8302-98096d221c00" />

---

## 📋 Table of Contents

- [Overview](#overview)
- [Dashboard Pages](#dashboard-pages)
  - [Budget Performance](#1-budget-performance)
  - [Sector Allocation & Spending](#2-sector-allocation--spending)
  - [Revenue Performance & Fiscal Adequacy](#3-revenue-performance--fiscal-adequacy)
- [Key Metrics & KPIs](#key-metrics--kpis)
- [Relationship Model](#relationship-model)
- [Dataset Schema](#dataset-schema)
- [File Structure](#file-structure)
- [Getting Started](#getting-started)
- [Usage & Filters](#usage--filters)

---

## Overview

The **Nigerian Budget Dashboard** is a Power BI report designed to make Nigeria's federal budget data accessible, transparent, and analytically actionable. It gives policymakers, budget analysts, journalists, researchers, and the general public a single interface for tracking how public funds are allocated and spent, identifying which sectors and MDAs (Ministries, Departments & Agencies) absorb the most resources, and evaluating whether government revenue is sufficient to cover expenditure obligations.

**Disclaimer: This project is intended for educational and analytical purposes only. The dataset used is modeled/simulated and does not represent the official approved Nigerian federal budget figures**

### 🎯 Business Objectives

- Monitor total budget expenditure, broken down by classification and expenditure type (Recurrent vs Capital)
- Track debt service obligations and evaluate their share of total spending
- Analyse how budget allocations are distributed across sectors and individual MDAs
- Identify the MDAs with the highest recurrent and capital spending concentration
- Assess revenue performance across all income streams (Main Pool, Independent Revenue, Grants & Special Levies, Other Revenue)
- Measure fiscal adequacy: how well revenue covers expenditure, and where gaps exist

---

## Dashboard Pages

### 1. Budget Performance

> *Tracks aggregate expenditure, debt service, recurrent vs capital split, and revenue-expenditure balance.*

<img width="1460" height="865" alt="Budget Performance Dashboard" src="https://github.com/user-attachments/assets/f91aca57-5b05-4f17-b5d4-7870eac2f111" />

#### KPI Cards

| KPI | Description |
|-----|-------------|
| **Total Expenditure** | Total budgeted or actual spending across all MDAs and budget heads |
| **Debt Service** | Total amount allocated or spent on servicing government debt |
| **Budget Surplus / Deficit** | Net fiscal position: Total Revenue minus Total Expenditure |
| **Recurrent** | Total recurrent (non-capital) expenditure |
| **Capital Budget** | Total capital (investment) expenditure |

#### Visuals

**Total Expenditure by Budget Classification : Clustered Column Chart**
- Compares spending across budget classifications (e.g. Personnel Costs, Overhead, Capital Projects, Debt Service)
- Reveals the structural composition of government spending and which classifications dominate the budget

**Expenditure by Type : Donut Chart**
- Splits total expenditure between Recurrent and Capital categories
- A high recurrent share signals limited investment in physical or social infrastructure

**Total Expenditure by Sector : Clustered Column Chart**
- Ranks all sectors (e.g. Education, Health, Infrastructure, Defence, Social Development) by their total expenditure
- Provides a top-level view of government spending priorities

**Revenue vs Expenditure : Donut Chart**
- Compares total revenue against total expenditure in a single visual
- Highlights the size of the fiscal gap or surplus

#### Slicers (available on all pages)

| Slicer | Field |
|--------|-------|
| Expenditure Type | Recurrent / Capital |
| Budget Classification | Classification label (e.g. Personnel, Overhead, Debt Service) |
| Budget Head | Specific budget head description |
| MDAs | Individual MDA names |
| Sector | Sector grouping of MDAs |
| Revenue Source | Individual revenue source name |

---

### 2. Sector Allocation & Spending

> *Analyses how budget resources are distributed across sectors and individual MDAs, with drill-down to entity level.*

<img width="1460" height="863" alt="Sector Budget Allocation   Spending Analytics Dashboard" src="https://github.com/user-attachments/assets/deecec0a-b7d4-47fe-b7f3-343d02d4ea0d" />

#### KPI Cards

| KPI | Description |
|-----|-------------|
| **Total MDAs** | Total number of Ministries, Departments & Agencies covered in the budget |
| **Top Sector (KPI)** | The sector with the highest total budget allocation |
| **Top MDA (KPI)** | The individual MDA with the highest total budget allocation |
| **Top 5% MDAs Share** | Share of total budget absorbed by the top 5% of MDAs — a concentration metric |

#### Visuals

**Recurrent Expenditure by Sector / MDA : Clustered Bar Chart** *(Drill down to MDA)*
- Displays recurrent spending ranked by sector, with drill-down to individual MDA level
- Identifies which sectors consume the most in personnel costs and overheads

**Capital Budget by Sector / MDA : Clustered Bar Chart** *(Drill down to MDA)*
- Displays capital allocations ranked by sector, with drill-down to individual MDA level
- Reveals where government investment spending is concentrated

**Sector & MDA Comparison Table : Pivot Table**
- Rows: MDA names; Columns: Recurrent, Capital Budget, Total
- Enables direct comparison of how each MDA's budget is split between recurrent and capital spending
- Supports sorting by any column to rank MDAs

**Total Expenditure by MDA : Clustered Bar Chart**
- Full horizontal bar ranking of all MDAs by their combined (recurrent + capital) expenditure
- Useful for identifying the dominant spenders in absolute terms

---

### 3. Revenue Performance & Fiscal Adequacy

> *Analyses all government revenue streams and measures how well they cover expenditure obligations.*

<img width="1459" height="865" alt="Revenue Performance   Fiscal Adequacy Dashboard" src="https://github.com/user-attachments/assets/3a921f20-7eee-4d96-985e-9a86e884152e" />

#### KPI Cards

| KPI | Description |
|-----|-------------|
| **Main Pool Revenue** | Revenue from the Federation Account / statutory allocations |
| **Total Revenue** | Aggregate revenue across all sources |
| **Independent Revenue** | Internally generated revenue (IGR) by MDAs |
| **Grants & Special Levies** | Revenue from grants, donor funding, and special levies |
| **Other Revenue** | All other revenue streams not captured in the above categories |

#### Visuals

**Total Revenue by Revenue Type / Source : Clustered Column Chart** *(Drill down to source)*
- Ranks revenue by type (e.g. Tax Revenue, Non-Tax Revenue, Grants), with drill-down to individual source
- Shows the structural breakdown of where government income originates

**Revenue by Source : Clustered Bar Chart**
- Horizontal bar ranking of individual revenue sources by total value
- Identifies the highest-contributing and most volatile revenue lines

**Fiscal Adequacy KPI Comparison : Clustered Column Chart**
- Plots key fiscal metrics (Total Revenue, Total Expenditure, Deficit/Surplus, Debt Service Coverage) side by side
- Directly answers the question: *"How sufficient is revenue in covering government obligations?"*
- Sourced from a dedicated KPI Table to support dynamic benchmarking

---

## Key Metrics & KPIs

| Metric | Definition |
|--------|-----------|
| **Total Expenditure** | Aggregate budget spend across all MDAs, classifications, and heads |
| **Recurrent Expenditure** | Non-capital government spending (personnel, overhead, debt service) |
| **Capital Budget** | Government investment spending on physical and social infrastructure |
| **Debt Service** | Amount set aside or spent on servicing domestic and external debt obligations |
| **Budget Surplus / Deficit** | Total Revenue minus Total Expenditure; positive = surplus, negative = deficit |
| **Total Revenue** | All government income: Main Pool, Independent, Grants, and Other Revenue |
| **Main Pool Revenue** | Statutory revenue from the Federation Account (FAAC allocations and similar) |
| **Independent Revenue** | Internally Generated Revenue (IGR) by individual MDAs |
| **Grants & Special Levies** | Donor grants, multilateral support, and designated levies |
| **Other Revenue** | Residual revenue lines not classified elsewhere |
| **Top Sector** | Sector with the highest aggregate budget allocation |
| **Top MDA** | Individual MDA with the highest budget allocation |
| **Top 5% MDAs Share** | Percentage of total budget captured by the highest-spending 5% of MDAs |
| **Total MDAs** | Count of distinct Ministries, Departments, and Agencies in the dataset |

---

## Relationship Model

| From (FK) | To (PK) | Join Column |
|-----------|---------|-------------|
| fact_expenditure.mda_key | dim_mda.mda_key | mda_key |
| fact_expenditure.category_key | dim_budget_category.category_key | category_key |
| fact_expenditure.head_key | dim_budget_head.head_key | head_key |
| fact_expenditure.fact_id | fact_revenue_projections.fact_id | fact_id |
| fact_revenue_projections.source_key | dim_revenue_source.source_key | source_key |

---

## Dataset Schema

### Fact Table

| Column | Type | Description |
|--------|------|-------------|
| `budget_head_id` | Integer (FK) | References dim_budget_head |
| `mda_id` | Integer (FK) | References dim_mda |
| `classification_id` | Integer (FK) | References dim_budget_category |
| `revenue_source_id` | Integer (FK) | References dim_revenue_source |
| `recurrent_amount` | Decimal | Recurrent budget allocation |
| `capital_amount` | Decimal | Capital budget allocation |
| `total_expenditure` | Decimal *(Calculated)* | Recurrent + Capital |
| `debt_service` | Decimal | Debt service component of the budget |
| `total_revenue` | Decimal | Total government revenue for the period |
| `budget_surplus` | Decimal *(Calculated)* | Total Revenue − Total Expenditure |

### Dimension Tables

**dim_mda**

| Column | Type | Description |
|--------|------|-------------|
| `mda_id` | Integer (PK) | Unique MDA identifier |
| `mda_name` | String | Full name of the Ministry, Department, or Agency |
| `mda_sector` | String | Sector the MDA belongs to (e.g. Education, Health, Infrastructure) |

**dim_budget_category**

| Column | Type | Description |
|--------|------|-------------|
| `classification_id` | Integer (PK) | Unique classification identifier |
| `classification` | String | Budget classification label (e.g. Personnel Costs, Capital Projects) |
| `expenditure_type` | String | Recurrent or Capital |

**dim_budget_head**

| Column | Type | Description |
|--------|------|-------------|
| `head_id` | Integer (PK) | Unique budget head identifier |
| `head_description` | String | Full description of the budget head |

**dim_revenue_source**

| Column | Type | Description |
|--------|------|-------------|
| `source_id` | Integer (PK) | Unique revenue source identifier |
| `source_name` | String | Name of the revenue source |
| `revenue_type` | String | Revenue type grouping (e.g. Tax Revenue, Non-Tax Revenue, Grants) |

### Calculated Measures (DAX)

| Measure Table | Measure | Description |
|---------------|---------|-------------|
| `Calculated Measures` | Total Expenditure | SUM of all budget expenditure |
| `Calculated Measures` | Recurrent | SUM of recurrent expenditure lines |
| `Calculated Measures` | Capital Budget | SUM of capital expenditure lines |
| `Calculated Measures` | Debt Service | SUM of debt service allocations |
| `Calculated Measures` | Budget Surplus | Total Revenue − Total Expenditure |
| `Calculated Measures` | Total Revenue | SUM of all revenue streams |
| `Calculated Measures` | Main Pool Revenue | Revenue from the Main Pool / Federation Account |
| `Calculated Measures` | Independent Revenue | Internally Generated Revenue (IGR) |
| `Calculated Measures` | Grants and Special Levies KPI | KPI measure for grants and levies revenue |
| `Calculated Measures` | Other Revenue | Revenue not classified in primary categories |
| `Calculated Measures` | Total MDAs | DISTINCTCOUNT of MDAs in scope |
| `Calculated Measures` | Top 5% MDAs Share | Share of total spend by top 5% of MDAs |
| `MDA KPIs` | Top 1 MDA Sector KPI | Highest-spending sector (formatted KPI label) |
| `MDA KPIs` | Top 1 MDA KPI | Highest-spending individual MDA (formatted KPI label) |

---

## File Structure

```
the-2026-nigerian-budget-dashboard/
│
├── 📊 The__Nigerian_Budget_Dashboard.pbix     # Main Power BI file
│
├── 📁 screenshots/
│   ├── Budget_Performance.png
│   ├── Sector_Allocation_and_Spending.png
│   └── Revenue_Performance_and_Fiscal_Adequacy.png
│
├── 📂 data/
│   └── Nigerian_Budget_Dataset.xlsx          # Source data file
│
└── 📄 README.md                                   # This file
```

---

## Getting Started

### Prerequisites

| Tool | Version | Purpose |
|------|---------|---------|
| [Power BI Desktop](https://powerbi.microsoft.com/desktop/) | Latest | Open & edit `.pbix` |
| Microsoft Excel | 2016+ | View / edit source dataset |

### Installation & Setup

1. **Clone or download the repository**
   ```bash
   git clone https://github.com/<your-username>/the-nigerian-budget-dashboard.git
   ```

2. **Open the dashboard**
   - Launch **Power BI Desktop**
   - Go to `File → Open` and select `The_Nigerian_Budget_Dashboard.pbix`

3. **Verify data source connection**
   - Navigate to `Home → Transform Data → Data Source Settings`
   - Update the file path to your local source dataset if prompted
   - Click `Close` and then `Refresh` to reload the data

4. **Refresh data**
   ```
   Home → Refresh
   ```

---

## Usage & Filters

The dashboard includes a collapsible slicer pane on all three pages. The following filters apply globally across every page:

| Slicer | Description |
|--------|-------------|
| **Expenditure Type** | Filter by Recurrent or Capital spending |
| **Budget Classification** | Filter by specific classification (e.g. Personnel Costs, DebtService)|
| **Budget Head** | Drill into a specific budget head line |
| **MDAs** | Focus on one or more specific Ministries, Departments & Agencies |
| **Sector** | Filter to a specific sector (e.g. Education, Health, Infrastructure) |
| **Revenue Source** | Isolate a specific government revenue stream |

### Navigation

Use the **left-hand page navigator** to switch between:
- `Budget Performance` — aggregate expenditure, debt, recurrent/capital split, and fiscal balance
- `Sector Allocation & Spending` — sector and MDA-level budget distribution and comparison
- `Revenue Performance & Fiscal Adequacy` — revenue streams, sources, and fiscal coverage analysis

Use the **RESET button** (top-right of each page) to clear all active slicer selections at once.
Use the **Filter icon** (top-right of each page) to open or collapse the slicer pane.

### Drill-Down Interactions

| Visual | Primary Level | Drill-Down Level |
|--------|--------------|-----------------|
| Recurrent by Sector | Sector | MDA |
| Capital Budget by Sector | Sector | MDA |
| Revenue by Type | Revenue Type | Revenue Source |

> **Tip:** Click the drill-down arrow in the top-right corner of any supporting visual to activate drill mode, then click a bar or column to go one level deeper. Use the **Up arrow** to return to the parent level.

---

## Author

**M1deTheAnalyst**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/m1detheanalyst)
[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github)](https://github.com/M1deTheAnalyst)
[![X](https://img.shields.io/badge/X-Follow-000000?style=for-the-badge&logo=twitter&logoColor=white)](https://x.com/M1deTheAnalyst)

---

*Built with ❤️ using Power BI | Promoting fiscal transparency and data-driven public sector accountability in Nigeria*
