# 🌍 Global Terrorism Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project performs a comprehensive Exploratory Data Analysis (EDA) on the **United Nations Global Terrorism Analysis (UNGTA) dataset**, which contains over **180,000 terrorist incidents** recorded worldwide from **1970 to 2017**.

The goal is to uncover patterns, trends, and insights that can help policymakers, security agencies, and humanitarian organizations make data-driven decisions in counter-terrorism strategy and conflict prevention.

---

## 📂 Dataset

- **Name:** Global Terrorism Data
- **Source:** United Nations Global Terrorism Analysis (UNGTA)
- **Records:** 180,000+ terrorist incidents
- **Time Period:** 1970 – 2017
- **File:** `Global Terrorism Data.csv`

### Key Features
| Column | Description |
|---|---|
| `iyear` | Year of incident |
| `country_txt` | Country where attack occurred |
| `region_txt` | Global region |
| `attacktype1_txt` | Type of attack (Bombing, Armed Assault, etc.) |
| `targtype1_txt` | Target category (Military, Civilian, Government, etc.) |
| `weaptype1_txt` | Weapon used |
| `gname` | Terrorist group name |
| `nkill` | Number of fatalities |
| `nwound` | Number of wounded |
| `success` | Whether the attack succeeded (1/0) |
| `suicide` | Whether it was a suicide attack (1/0) |

---

## 🎯 Business Objective

To provide the United Nations and affiliated organizations with actionable, evidence-based insights that help:
- Allocate counter-terrorism resources efficiently
- Identify high-risk regions and emerging hotspots
- Understand the most lethal attack types and groups
- Support policy decisions that protect civilian populations

---

## 🛠️ Libraries Used

```python
import pandas as pd       # Data manipulation and aggregation
import numpy as np        # Numerical operations
import matplotlib.pyplot as plt  # Core visualizations
import seaborn as sns     # Statistical visualizations
```

---

## 📊 Analysis Structure (UBM Framework)

### 1. Know Your Data
- Dataset shape, info, data types
- Duplicate and missing value analysis

### 2. Understanding Variables
- Column descriptions and unique value counts
- Statistical summary

### 3. Data Wrangling
- Column selection and renaming
- Missing value imputation
- Outlier detection and winsorization
- Feature engineering (`decade`, `era`, `intensity`, `is_lethal`, `total_casualties`)

### 4. Visualizations (21 Charts)

#### 🔵 Univariate Analysis
| # | Chart | Type |
|---|---|---|
| 1 | Yearly attack frequency | Line Chart |
| 2 | Attacks by region | Horizontal Bar |
| 3 | Attack type distribution | Donut Chart |
| 4 | Weapon type frequency | Bar Chart |
| 5 | Fatality distribution | Histogram + Box Plot |

#### 🟡 Bivariate Analysis
| # | Chart | Type |
|---|---|---|
| 6 | Attacks over time by region | Stacked Area |
| 7 | Average fatalities by attack type | Bar Chart |
| 8 | Top 20 most affected countries | Bar Chart |
| 9 | Monthly seasonality of attacks | Bar Chart |
| 10 | Attack success rate by type | Grouped Bar |
| 11 | Top 15 deadliest terrorist groups | Bar Chart |
| 12 | Suicide vs non-suicide lethality | Box Plot |
| 13 | Killed vs Wounded relationship | Scatter Plot |

#### 🔴 Multivariate Analysis
| # | Chart | Type |
|---|---|---|
| 14 | Correlation between numerical features | Heatmap |
| 15 | Pairwise variable relationships | Pair Plot |
| 16 | Attacks by region and decade | Heatmap |
| 17 | Fatalities by region and decade | Grouped Bar |
| 18 | Attack type vs target type | Crosstab Heatmap |
| 19 | Lethality by era and attack type | Pivot Heatmap |
| 20 | Attack volume vs fatalities by region | Bubble Chart |
| 21 | Top 10 countries by total deaths | Bar Chart |

---

## 💡 Key Insights

- Global terrorism **peaked around 2014** during ISIS's territorial expansion
- **Middle East & North Africa** and **South Asia** account for ~50% of all attacks
- **Bombing/Explosion** is the most common attack type (~50% of incidents)
- **Suicide attacks**, though only ~2–3% of attacks, are **5–8x more lethal** per incident
- **ISIS, Taliban, and Boko Haram** are the deadliest groups by total fatalities
- **Western Europe's decline** in terrorism since the 1990s proves sustained counter-terrorism works
- Attack lethality is **increasing over time** — modern attacks kill more per incident than historical ones

---

## ✅ How to Run

1. Clone this repository
   ```bash
   git clone https://github.com/your-username/Global-Terrorism-EDA.git
   cd Global-Terrorism-EDA
   ```

2. Place `Global Terrorism Data.csv` in the same folder as the notebook

3. Install required libraries
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

4. Open and run the notebook
   ```bash
   jupyter notebook Global_Terrorism_EDA.ipynb
   ```

> **Google Colab users:** Upload the CSV using the file upload cell provided at the top of the notebook.

---

## 📁 Repository Structure

```
Global-Terrorism-EDA/
│
├── Global_Terrorism_EDA.ipynb   # Main EDA notebook
├── Global Terrorism Data.csv    # Dataset (download separately)
└── README.md                    # Project documentation
```

---

## 👤 Author

**Prince Rathore**
- GitHub: [@princerathore981](https://github.com/princerathore981)

---

## 📄 License

This project is for educational purposes as part of an EDA Capstone submission.
