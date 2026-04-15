# Manufacturing-Production-Dashboard-Power-BI
## 📊 Project Overview
A comprehensive **Manufacturing Analytics Dashboard** built with Power BI, featuring star schema design, 500+ fact records, and interactive KPIs for production monitoring.

![Dashboard Preview](dashboard_preview.png)

## 🎯 Key Features
- ✅ **Star Schema Design** (1 Fact Table + 5 Dimension Tables)
- ✅ **500 Production Records** (Realistic manufacturing data)
- ✅ **5 Dashboard Pages** with 25+ interactive visuals
- ✅ **25 DAX Measures** including OEE, MTBF, Defect Rate
- ✅ **Dynamic Card Colors** based on KPI performance

## 📁 Data Model
DimDate ──┐
DimProduct ──┤
DimMachine ──┼── FactProduction
DimShift ──┤
DimEmployee ──┘

text

## 📈 Dashboard Pages
| Page | Focus | Key Metrics |
|------|-------|-------------|
| 1 | Executive Dashboard | OEE, Production Trend, MTBF |
| 2 | Production Analysis | Cycle Time, Utilization |
| 3 | Quality & Defects | Defect Rate, First Pass Yield |
| 4 | Machine & Downtime | Availability, MTTR |
| 5 | Employee Performance | Productivity by Shift |

## 🔧 DAX Measures Included
```dax
// Core Manufacturing KPIs
OEE = [Availability] * [Performance] * [Quality]
MTBF = DIVIDE([Total Cycle Time], COUNTROWS(FILTER(...)))
Defect Rate = DIVIDE([Total Defects], [Total Produced])
🚀 How to Use
Download all CSV files from /data folder

Open Power BI Desktop

Load CSVs and establish relationships
