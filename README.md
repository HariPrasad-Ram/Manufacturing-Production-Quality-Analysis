# 🏭 Manufacturing Production & Quality Analysis Dashboard  

## 📊 Project Objective  
The primary objective of this project is to analyze manufacturing performance data to monitor key production metrics, 
identify inefficiencies, and improve product quality. The dashboard provides actionable insights into daily production trends,
rejection analysis, employee performance, and machine efficiency to support data-driven decision-making for optimizing production processes and reducing wastage.

---

## 🧾 Dataset Used  
- **Source:** Manufacturing production dataset (SQL + Excel format)  
- **Imported Using:** SQL Queries for KPI extraction and Tableau for visualization  
- **Duration:** January 2015 – September 2015  
- **Tools Used:**  
  - SQL (for KPI computation and data preparation)  
  - Tableau (for interactive dashboards)  
  - Excel (for raw data cleaning and verification)  

---

## 🗝️ Key Metrics (KPIs)  

| KPI | Description | Query Logic / Measure |
|-----|--------------|------------------------|
| **Total Manufactured Quantity** | Total items produced during the period | `SUM(Today Manufactured Qty)` |
| **Total Processed Quantity** | Quantity processed in the production line | `SUM(Processed Qty)` |
| **Total Rejected Quantity** | Items rejected due to quality issues | `SUM(Rejected Qty)` |
| **Wastage Percentage** | Percentage of rejected items vs processed | `(Rejected Qty / Processed Qty) * 100` |
| **Employee-wise Rejected Qty** | Identifies employees contributing most to rejections | `GROUP BY Emp Name` |
| **Machine-wise Rejected Qty** | Highlights machines causing high rejection rates | `GROUP BY Machine Code` |
| **Average Daily Production** | Average production per day | `AVG(Produced Qty)` |

---

## ⚙️ Process Workflow

1. **Data Import & Cleaning**
   - Imported dataset into SQL and Tableau.
   - Handled missing/blank fields, standardized column names.
   - Validated consistency between production and rejection records.

2. **Data Transformation & KPI Calculations**
   - Used SQL queries to compute KPIs (see SQL script for full logic).
   - Created measures for production efficiency, rejection %, and employee/machine performance.

3. **Dashboard Development**
   - Built interactive Tableau dashboard with filters for Department, Employee, and Machine.
   - Visualized month-wise production trends and rejection comparisons.
   - Designed cards and charts for better interpretability (bar, trendline, and KPI boxes).

---

## 🧩 Dashboard Overview (Tableau)  

- **Department-wise Analysis:**  
  Compared total manufactured vs rejected quantity across departments like *Footwear, Knitwear, Printed Fabric,* and *Woven Labels*.

- **Operation-wise Rejection:**  
  Identified highest rejection in “Cut & Fold” and “Printing” operations.

- **Employee-wise Rejection:**  
  Highlighted top 4 employees with maximum rejected quantities (e.g., Shruti Singh, Pooja Patel).

- **Machine Performance:**  
  Machine codes *MC106* and *MC095* recorded highest rejection rates.

- **Production Trends:**  
  Monthly analysis revealed a consistent output of **~5M units per quarter** with slight dips during mid-year.

- **Key Observation:**  
  Despite strong production volume (~60M units), rejection reached **0.49M**, leading to a **0.82% wastage rate**, indicating room for process improvement.
<img width="1294" height="730" alt="Screenshot 2025-10-19 110418" src="https://github.com/user-attachments/assets/bcd914a2-5eb7-420d-b268-03368a9c0ecc" />
<img width="1336" height="735" alt="Screenshot 2025-10-19 110719" src="https://github.com/user-attachments/assets/0ea90c0b-d53e-424e-ac53-6962f5f4291e" />
<img width="979" height="656" alt="Screenshot 2025-10-19 110818" src="https://github.com/user-attachments/assets/623a9fe5-ff5b-4387-b6dd-608b21202aa1" />
<img width="1170" height="619" alt="Screenshot 2025-10-19 111002" src="https://github.com/user-attachments/assets/64a912fb-bd63-46c6-b065-1753d651a9ab" />

---

## 🧠 Insights & Recommendations

- Optimize underperforming machines (e.g., MC095, MC106) through maintenance and calibration.  
- Provide quality training to employees with consistently higher rejection rates.  
- Reassess workflow in “Cut & Fold” and “Printing” operations.  
- Introduce automated inspection systems to reduce manual errors.  
- Continue tracking KPIs weekly for early anomaly detection.

---

## 🛠️ Technical Stack

| Tool | Purpose |
|------|----------|
| **SQL** | KPI calculation, data validation |
| **Tableau** | Dashboard creation and visualization |
| **Excel** | Initial data cleaning and validation |
| **Power BI (Optional)** | Cross-platform visualization comparison |

---

## 📂 Repository Structure

```
📁 Manufacturing-Analysis
│
├── 📄 README.md
├── 📊 manufacturing_analysis.pbix
├── 📈 tableau_updated_project_pdt.pdf
├── 💾 Dataset_SQL.sql
└── 📘 dataset.xlsx (if available)
```

---

## 📌 Key Outcomes

- Achieved clear visibility into production efficiency and rejection causes.  
- Identified high-impact problem areas across departments, machines, and employees.  
- Delivered interactive Tableau and Power BI dashboards for ongoing monitoring.  
- Enabled data-driven strategies for improving manufacturing quality.

---

### 👤 Author  
**Hari Prasad Ram**  
📧 [LinkedIn](https://www.linkedin.com/in/hariprasad-ram-933152358/) | [GitHub](https://github.com/HariPrasad-Ram)  

---
