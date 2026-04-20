# 🔍 AI-Assisted Customer Transaction Analysis

> **Mid-Project | AI Advanced Data Analyst Track — Global Knowledge**

A complete data analysis pipeline applied to a real-world retail transaction dataset (~20,800 records), covering data cleaning, feature engineering, and business insight generation — with AI-assisted prompt engineering as part of the methodology.

---

## 📌 Project Objectives

1. **Exploratory Data Analysis (EDA)** — Understand distributions, patterns, and anomalies
2. **Data Cleaning** — Resolve missing values, typos, and inconsistencies
3. **Data Quality Validation** — Ensure integrity before analysis
4. **Feature Engineering** — Derive meaningful variables from raw fields
5. **Insight Generation** — Produce 5 targeted visualizations with business conclusions

---

## 📂 Dataset

| File | Description |
|------|-------------|
| `module3_4_full_demo_dataset.csv` | Raw dataset (20,800 transactions) |
| `Result.csv` | Cleaned & processed output (19,656 records) |

**Features:** `transaction_date`, `customer_id`, `region`, `product_category`, `units_sold`, `unit_price`, `revenue`, `high_value`

---

## 🧹 Data Quality Issues Found & Fixed

| Issue | Detail | Resolution |
|-------|--------|------------|
| Missing values — `region` | 3,971 nulls (19%) | Flagged as `"Unknown"` |
| Missing values — `revenue` | 523 nulls | Rows removed |
| Typo in `product_category` | `"Clothng"` → `"Clothing"` | Standardized |
| Inconsistent casing in `region` | `"north"` / `"North"` | Normalized to title case |
| Date format | Datetime with time component | Stripped to date only |
| Total rows removed | 1,144 rows (~5.5%) | After all cleaning steps |

---

## 📊 Visualizations & Insights

### 1. Correlation Heatmap of Customer Behaviors
Explored relationships between `units_sold`, `unit_price`, `revenue`, and `high_value` to identify which variables drive high-value transactions.

### 2. Scatter Plot: Frequency vs. Spend
Mapped customer purchase frequency against total spend to segment behavioral clusters — foundation for RFM-style analysis.

### 3. Bar Chart: Revenue by Product Category
Compared revenue performance across categories (Beauty, Clothing, Home, Sports, Electronics) to identify top-performing segments.

### 4. Boxplot: Transaction Revenue Distribution by Region
Revealed regional revenue spread and outliers — highlighting which regions have the highest variability in transaction value.

### 5. Histogram: Customer Recency Distribution
Analyzed how recently customers made purchases to identify active vs. at-risk customer segments.

---

## 🤖 AI-Assisted Methodology

This project intentionally incorporates **prompt engineering as a core skill**. AI tools were used to:
- Accelerate EDA hypothesis generation
- Validate cleaning logic
- Suggest feature engineering approaches

> Knowing *how* to prompt an AI model effectively — with domain context, clear constraints, and critical evaluation of outputs — is a professional skill in modern data workflows.

All prompts used are included in [`prompts/`](./prompts/) for full transparency.

---

## 🛠️ Tools & Libraries

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn`

---

## 👤 Author

**Ziad Mohamed Gomaa Afifi**
Computer Science, Ain Shams University — Class of 2026
[LinkedIn](https://www.linkedin.com/in/ziad-mohamed-23b318327)
