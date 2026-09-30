# Exponential Data Analysis on the CMS Open Payments Dataset

A large-scale exploratory and statistical analysis of the **CMS Open Payments dataset (2019–2025)** containing approximately **87.7 million reported payment records and 91 variables**.

The project investigates payment distributions, categorical relationships, temporal trends, geographic concentration, statistical associations, hypotheses, and the robustness of the observed findings.

---

## Overview

The CMS Open Payments dataset contains reported payments and transfers of value made by applicable manufacturers and applicable group purchasing organizations (GPOs) to covered recipients.

This project performs a comprehensive analysis of the dataset using a combination of:

- Exploratory Data Analysis
- Data-quality analysis
- Distribution analysis
- Bivariate analysis
- Multivariate analysis
- Time-series analysis
- Geographic analysis
- Statistical hypothesis testing
- Effect-size analysis
- Sensitivity and robustness analysis

The analysis was designed specifically for a very large dataset, with approximately **87.7 million valid payment records**.

---

## Key Questions

The analysis investigates questions such as:

- How are payment amounts distributed?
- How concentrated are payments among small and large transactions?
- Which payment categories are associated with different payment amounts?
- How are payment types related to recipient types?
- How are product categories related to product types?
- Does the number of payments relate to the total payment amount?
- How has payment activity changed from 2019 to 2025?
- Did payment activity change substantially around 2020?
- How did typical payment amounts change over time?
- How geographically concentrated are reported payments?
- Are the observed relationships robust to different samples, periods, transformations, and cleaning choices?

---

# Dataset

### Source

The underlying data comes from the **U.S. Centers for Medicare & Medicaid Services (CMS) Open Payments Program**.

The original dataset is not included in this repository because of its very large size.

The official CMS source should be used to obtain the data required to reproduce the analysis.

**Official source:**  
https://openpaymentsdata.cms.gov/datasets

---

## Data Ownership and Attribution

The underlying dataset is provided by the **U.S. Centers for Medicare & Medicaid Services (CMS)** through the Open Payments Program.

The dataset is not created or owned by the author of this project.

This repository contains independent analysis, visualizations, statistical calculations, interpretations, and documentation performed on the publicly available data.

This project is not an official CMS analysis and does not represent CMS endorsement of the analysis or its conclusions.

---

# Dataset Scope

| Property | Value |
|---|---:|
| Program years | **2019–2025** |
| Reported records | **~87.7 million** |
| Variables | **91** |
| Primary numerical variables | Payment Amount, Number of Payments |
| Temporal variables | Payment Date, Program Year |
| Geographic variables | Recipient and payment-making entity locations |
| Dataset type | Large-scale tabular financial/payment data |

---

# Technology Stack

The analysis was performed in Python using:

| Library | Purpose |
|---|---|
| **Polars** | Large-scale dataframe processing and LazyFrame operations |
| **NumPy** | Numerical computation |
| **SciPy** | Statistical analysis and hypothesis testing |
| **Matplotlib** | Data visualization |
| **GeoPandas** | Geographic analysis and mapping |

The analysis uses **Polars LazyFrame** operations to work efficiently with the large dataset.

---

# Analysis Workflow

The notebook follows a structured analytical workflow:

```text
Data Source
    ↓
Data Loading
    ↓
Data Quality Analysis
    ↓
Univariate Analysis
    ↓
Bivariate Analysis
    ↓
Multivariate Analysis
    ↓
Time-Series Analysis
    ↓
Distribution Analysis
    ↓
Statistical Testing
    ↓
Hypothesis Testing
    ↓
Sensitivity & Robustness Analysis
    ↓
Final Findings
