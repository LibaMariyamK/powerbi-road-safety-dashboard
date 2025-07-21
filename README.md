# 🚦 Addis Ababa Road Safety Dashboard (2017–2020)

An interactive Power BI dashboard that analyzes road accident and casualty data from Addis Ababa between 2017 and 2020. This project focuses on uncovering trends related to accident severity, affected groups, vehicle involvement, and key causes — backed by thoughtful data cleaning and relationship modeling.

---

## 📁 Dataset

- **Dataset CSV File in this repo**: [RTA Dataset.csv](https://github.com/LibaMariyamK/EDA-Road-Traffic-Accidents/blob/main/RTA%20Dataset.csv)
- **Issue**: Casualty-related columns had a high percentage of missing values.
- **Solution**: I split the original dataset into two related tables:
  - `road_saftey`: Core accident data (retained full records)
  - `casualty_info`: Casualty-specific data (records with non-null values)
  - Linked both using the common `Record_ID` field to maintain referential integrity and avoid excessive data loss.

---

## 🧼 Data Cleaning Highlights

- Removed nulls from casualty-related columns **only in the separate table**, preserving full accident details
- Handled inconsistent data types and removed duplicates
- Created calculated columns and measures using **DAX**
- Defined relationships between tables using `Record_ID` in Power BI’s data model

---

## 📊 Dashboard Overview

| Page | Description |
|------|-------------|
| **1. Road Safety Overview** | Total accidents, injuries by type, age-group insights |
| **2. Casualty Breakdown** | Total casualties, fatalities, work types, and child involvement |
| **3. Vehicle & Cause Analysis** | Vehicle types vs. fatalities and major contributing causes |
| **4. Executive Summary** | Key stats, major insights, and actionable recommendations |

> 🖼️ A PDF version of the final dashboard is included in this repo: [`dashboard_summary.pdf`](./RTA.pdf)

---

## 📌 Key Insights

- 👨‍🦱 **Drivers aged 18–30** are involved in more than 50% of all accidents
- 🚛 **Lorries** are the top vehicle in total and fatal accidents
- ⚠️ **Slight injuries** make up over 84% of accident outcomes
- 👷‍♂️ **Drivers and riders** are the most affected in casualty data
- 🚸 Over **10% of total casualties** involve children under 18

---

## 💡 Recommendations

- Implement targeted safety programs for young drivers and commercial vehicle operators
- Enforce rules on lane discipline and vehicle spacing
- Introduce protective policies in school zones
- Mandate periodic health and safety training for high-risk job roles

---

## 🧰 Tools Used

- **Power BI Desktop**
- **Power Query** (data transformation)
- **DAX** (measures and calculated columns)
- **Excel** (initial file inspection)

---


## 📌 How to Use

1. Clone or download this repository
2. Open the `.pbix` file in Power BI Desktop
3. Explore the report using filters, slicers, and page navigation
4. View the PDF if you don’t have Power BI installed

---

