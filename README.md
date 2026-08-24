# 📦 QuickCart Warehouse Inventory Stockout Risk Prediction

### Multi-Table Classification for Predicting Safe / At-Risk / Imminent Inventory

A machine learning project that predicts stockout risk for every **SKU, store, and day** using inventory, demand, supplier, store, and event-related information.

The project was developed as part of a machine learning internship project and focuses on a realistic operational inventory-management problem.

---

## 📌 Project Overview

Quick-commerce businesses need to maintain product availability while avoiding unnecessary overstocking.

The key business question addressed in this project is:

> **For every product, in every store, on every day — will the product run out of stock before the next supplier delivery arrives?**

The system classifies each inventory record into one of three categories:

| Risk Level | Description |
|---|---|
| 🟢 Safe | Sufficient stock coverage beyond the replenishment requirement |
| 🟡 At-Risk | Inventory coverage is close to the replenishment requirement |
| 🔴 Imminent | Stock may run out before the next supplier delivery |

---

## 🎯 Objectives

- Integrate multiple inventory-related datasets
- Clean and preprocess relational data
- Perform exploratory data analysis
- Engineer inventory and demand-related features
- Build multi-class classification models
- Compare different machine learning approaches
- Identify important stockout-risk factors
- Analyse festival and category-level risk
- Generate actionable business recommendations

---

## 🗂️ Dataset

The project uses five interconnected tables.

| Dataset | Rows | Description |
|---|---:|---|
| `dim_stores.csv` | 12 | Store information |
| `dim_skus.csv` | 60 | Product/SKU information |
| `dim_suppliers.csv` | 15 | Supplier information |
| `dim_events.csv` | 30 | Festival and promotional events |
| `fact_inventory_daily.csv` | 21,600 | Daily inventory records |

### Dataset Dimensions

- **12 stores**
- **60 SKUs**
- **15 suppliers**
- **30 days**
- **21,600 inventory records**
- **8 product categories**

The 21,600 records represent:

```text
12 stores × 60 SKUs × 30 days = 21,600 records
