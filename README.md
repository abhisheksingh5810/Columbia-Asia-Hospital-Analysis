# Columbia Asia Hospital - Data Analytics & Business Intelligence Dashboard


## 📊 Project Overview

A comprehensive **healthcare data analytics and business intelligence capstone project** that demonstrates end-to-end data analysis, visualization, and optimization capabilities. This project analyzes hospital operations data from Columbia Asia Hospital including patient demographics, doctor performance metrics, department efficiency, and patient satisfaction trends.

**Key Achievement:** Delivered actionable insights from 15,000+ patient records with 72% data quality challenges resolved through statistical imputation and advanced data cleaning techniques.

---

## 🎯 Key Features & Analysis

### 📈 Patient Analytics
- **Demographic Segmentation** - Analyzed patient visits across 5 age groups:
  - Children (0-18 years)
  - Young Adults (18-30 years)
  - Middle-Aged Adults (30-50 years) - **Highest utilization**
  - Older Adults (50-70 years)
  - Elderly (70+ years)

- **Gender Distribution Analysis** - Gender-based patient patterns:
  - Male Patients: 4,705 (45.4%)
  - Female Patients: 4,487 (43.4%)
  - Not Categorized: 24 (0.2%)

- **Patient Satisfaction Scoring** - Correlation analysis between wait times, demographics, and satisfaction scores with dynamic updates based on thresholds

### 🏥 Department Performance Metrics
- **Visit Volume Analysis** - General Practice department leading with 7,240+ visits
- **Departmental Efficiency** - Waiting time optimization and performance trending
- **Gender-Based Billing Ratios** - Revenue analysis by gender per department

### 👨‍⚕️ Doctor Performance Dashboard
- **Revenue Generation Analysis** - Top 5 revenue-generating doctors identified
- **Patient Satisfaction Correlation** - Average satisfaction scores by doctor
- **Patient Diversity Metrics** - Racial and demographic diversity of each doctor's patient base
- **Doctor Gender Ratios** - Patient gender distribution analysis by healthcare provider

### ⏱️ Operational Insights
- **Average Waiting Time** - 35.26 minutes (overall average)
- **Wait Time Trends** - Identified departments with consecutive months of decreasing wait times
- **Efficiency Optimization** - Performance trending and benchmarking across departments

---

## 🛠️ Technologies & Tools

| Technology | Purpose | Details |
|-----------|---------|---------|
| **Power BI** | Interactive Dashboards | 3-tab dashboard (Main, Doctors', Patients') with dynamic visualizations |
| **SQL** | Data Analysis & Querying | 21 complex queries using CTEs, window functions, and aggregations |
| **DAX** | Advanced Calculations | Dynamic KPI formulas and conditional logic |
| **Data Cleaning** | Quality Assurance | Handled missing values, format standardization, and validation |
| **Excel** | Data Source | Original datasets: Doctor_Patients_data, Hospital_ER tables |

---

## 📁 Project Deliverables

### 1. **Power BI Interactive Dashboard** (`Columbia_Asia_Hospital_PowerBI_Dashboard.pbix`)
   - **Main Tab** - Overall hospital metrics and KPIs
   - **Doctors' Tab** - Doctor performance, satisfaction scores, revenue metrics
   - **Patients' Tab** - Patient demographics, visit patterns, satisfaction analysis
   - Real-time filtering and drill-down capabilities

### 2. **SQL Query File** (`HOSPITAL_SQL_QUERY_abhi.sql`)
   - **21 Complex Queries** addressing business questions:
     - Q15: Top 5 revenue-generating doctors with fewest patients
     - Q16: Average waiting time decrease over consecutive months
     - Q17: Doctor gender ratio analysis
     - Q18: Average satisfaction score by doctor
     - Q19: Doctors with diverse patient demographics
     - Q20: Male-to-Female billing ratios per department
     - Q21: Patient satisfaction score updates (conditional logic)

### 3. **Comprehensive Documentation** (`Columbia_Asia_Hospital__docx_abhi.docx`)
   - Answers to 21 objective questions with detailed methodology
   - Solutions to 14 subjective questions
   - Data cleaning approach and rationale
   - DAX formulas and query explanations
   - Visual evidence and screenshots

### 4. **Presentation Deck** (`Columbia_Asia_Hospital_PPT__resub.pptx`)
   - 16 slides with key findings and visualizations
   - Executive summary with actionable insights
   - Data cleaning methodology
   - Performance metrics and trends

---

## 📊 Key Metrics & Findings

### Data Quality Management
- **Null Values Handled:** 72% of patient satisfaction scores (replaced with statistical average)
- **Data Cleaning Success Rate:** 100% data consistency achieved
- **Records Processed:** 15,000+ patient visit records

### Performance Indicators
- **Average Patient Wait Time:** 35.26 minutes
- **Most Visited Department:** General Practice (7,240 visits)
- **Patient Gender Distribution:** 4,705 M : 4,487 F
- **Age Group Utilization:** 30-50 age group (Middle-Aged Adults) shows highest healthcare service usage

### Business Insights
- Gender-based billing disparities identified across departments
- Doctor satisfaction scores correlate with patient demographic diversity
- Wait time reduction trends enable department optimization
- Revenue concentration identified among top 5 doctors



## 🔧 Technical Implementation

### Data Cleaning Approach
```
Challenge: 72% null values in patient satisfaction scores
Solution: Statistical imputation using average values
Rationale: High volume prevented data elimination
Result: Maintained data integrity while filling gaps
```

### DAX Formula Example
```DAX
Average Wait Time = AVERAGE('Hospital ER'[patient_waittime])
Visit By Department Referral = CALCULATE(COUNTROWS('Hospital ER'), 
    GROUPBY('Hospital ER','Hospital ER'[department_referral]))
```

### SQL Query Complexity
- **Window Functions:** LEAD(), ROW_NUMBER() for sequential analysis
- **CTEs (Common Table Expressions):** Multi-step logic for waiting time trends
- **Conditional Logic:** CASE statements for dynamic score calculations
- **Aggregations:** SUM(), COUNT(), AVG() with GROUP BY and HAVING clauses

---

## 📈 Analytics Capabilities Demonstrated

✅ **Data Cleaning & Preparation** - Handled missing values and format standardization  
✅ **Statistical Analysis** - Trend analysis, averages, ratios, correlations  
✅ **SQL Mastery** - Complex queries with advanced functions and optimization  
✅ **DAX Programming** - Dynamic KPI calculations and conditional logic  
✅ **Data Visualization** - Interactive dashboards with drill-down capabilities  
✅ **Business Acumen** - Identified actionable insights and optimization opportunities  
✅ **Documentation** - Comprehensive methodology and technical explanations  
✅ **Stakeholder Communication** - Executive summaries and visual presentations  

---

## 📋 Requirements & Dependencies

- **Power BI Desktop** (2023.x or later) or Power BI Service access
- **SQL Server/MySQL** (for running SQL queries)
- **Microsoft Word** (for viewing documentation)
- **Microsoft PowerPoint** (for viewing presentation)
- Original datasets: `Doctor_Patients_data.xlsx` and `Hospital_ER.xlsx`

---

## 🎓 Learning Outcomes

This project demonstrates proficiency in:
- Healthcare data analytics and operational metrics
- Advanced SQL query writing (CTEs, Window Functions, Aggregations)
- Power BI dashboard design and DAX formula creation
- Data cleaning and handling missing values
- Statistical analysis and trend identification
- Business intelligence and reporting
- Professional documentation and presentations

---

## 📂 File Structure

```
Columbia-Asia-Hospital-Analytics/
├── README.md (this file)
├── Columbia_Asia_Hospital_PowerBI_Dashboard.pbix
├── Columbia_Asia_Hospital__docx_abhi.docx
├── Columbia_Asia_Hospital_PPT__resub.pptx
├── HOSPITAL_SQL_QUERY_abhi.sql
└── DATA/
    ├── Doctor_Patients_data.xlsx
    └── Hospital_ER.xlsx
```


## 💡 Key Insights & Recommendations

### For Operations Team
- Focus on wait time reduction in General Practice department
- Implement satisfaction score improvements for long wait times (>30 min)
- Monitor consecutive month trends for performance optimization

### For Doctor Management
- Recognize top 5 revenue-generating doctors
- Address satisfaction score gaps for specific demographics
- Leverage diverse patient exposure as training opportunity

### For Administrative Planning
- Allocate resources based on age group utilization patterns
- Address gender-based billing disparities
- Implement demographic-specific patient care strategies


## ⭐ Highlights

- **15,000+ Records Analyzed** with 72% data quality challenges resolved
- **21 Complex SQL Queries** demonstrating advanced database skills
- **Interactive 3-Tab Dashboard** with drill-down capabilities
- **100% Data Integrity** achieved through scientific imputation methods
- **Comprehensive Documentation** with methodology and visual evidence
- **Executive Presentation** with actionable insights

---
