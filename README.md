# bengaluru-rental-eda
EDA &amp; KPI Analysis of 1200+ Bengaluru Rental Records.   
# Bengaluru Rental Market - EDA & KPI Analysis
### Data Analyst Project by Hajira Shaikh | Bengaluru, India

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📊 Project Overview
Exploratory Data Analysis of 1200+ Bengaluru rental properties to identify trends, validate data quality, and calculate key business KPIs. This project demonstrates core Data Analyst skills: data cleaning, EDA, KPI validation, and actionable insights.

**Key Question:** Which areas, BHK types, and sizes drive rental pricing in Bengaluru?

## 🎯 Skills Demonstrated
- **Data Cleaning:** Handled 12.5% missing values, duplicates, outliers
- **Data Quality Checks:** Profiled distributions, missing patterns
- **EDA & Trend Analysis:** Correlation, grouping, pattern identification
- **KPI Validation:** Avg Rent, Rent/sqft, Demand Distribution
- **Visualization:** Matplotlib - Bar, Scatter, Pie charts
- **Tools:** Python, Pandas, NumPy, Matplotlib, Jupyter

## 📁 Dataset
`bengaluru_rental_data.csv` (1200 records)
- **Features:** Area, BHK, Size_sqft, Rent_INR, Age_years, Furnishing
- **Source:** Synthetic dataset modeled on real Bengaluru market
- **Quality Issues Intentionally Added:** Missing values, outliers for cleaning practice

## 🔍 Key Findings & Business Insights

### 1. Data Quality Issues Found
- **12.5% missing** Rent values → Fixed with median imputation by BHK group
- **6.6% missing** Furnishing → Filled as 'Unknown'
- **Outliers in Size:** Filtered to 500-3000 sqft range

### 2. KPI - Average Rent by Area
- **Premium Areas:** Koramangala (₹25,866), Jayanagar (₹25,445), Indiranagar (₹25,323)
- **Affordable:** BTM Layout (₹24,036), HSR Layout (₹24,112)
- **Insight:** Central premium locations command 7-8% higher rent

### 3. Trend - Rent vs Size
- **Correlation:** 0.18 (weak positive) - Size alone doesn't drive rent in Bengaluru
- **Pattern:** Area and Furnishing matter more than just size
- **Insight:** Location premium > Size premium

### 4. KPI - Market Demand by BHK
- **2 BHK:** 49.3% - Highest demand (mid-size families, working couples)
- **1 BHK:** 30.5% - Single professionals
- **3 BHK:** 20.2% - Premium segment

### 5. Business Recommendation
> **Focus on 2BHK in HSR/Whitefield:** High demand (50%), moderate rent, good ROI for investors. 1BHK in BTM/Marathahalli for affordable segment.

## 📈 Visualizations
### Avg Rent by Area
![Avg Rent](chart1_avg_rent.png)

### Rent vs Size Trend
![Rent vs Size](chart2_rent_vs_size.png)

### BHK Demand Distribution
![BHK](chart3_bhk.png)

## 💻 How to Run
```bash
pip install pandas matplotlib
python bengaluru_eda_analysis.py