# HR Analysis Dashboard | Power BI

## 📊 Project Overview

The **HR Analysis Dashboard** is an interactive Power BI project designed to analyze employee demographics, workforce distribution, hiring patterns, department-level attrition, employee status, and job-title distribution.

The dashboard provides HR stakeholders with a single view of key workforce KPIs and enables department-level filtering through an interactive **Department slicer**.

---

## 🎯 Business Problem

HR teams often have employee information spread across different views, making it difficult to quickly answer questions such as:

- How large is the current workforce?
- What percentage of employees work from headquarters versus remotely?
- What is the current attrition rate?
- Which departments have the largest employee populations?
- Which departments show higher numbers of terminated employees?
- How has the employee hiring mix changed over the years?
- What is the workforce distribution by race?
- Which job titles have the largest employee populations?
- What proportion of employees are active versus terminated?

This dashboard brings these questions together in one interactive reporting solution.

---

## 🎯 Project Objectives

1. Build an interactive HR analytics dashboard in Power BI.
2. Create KPI cards for important workforce metrics.
3. Analyze hiring distribution by year.
4. Compare employee and termination counts by department.
5. Understand workforce composition by race.
6. Analyze active versus terminated employees.
7. Identify the most populated job titles.
8. Enable department-level filtering for interactive analysis.
9. Present HR information in a management-friendly format.

---

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **Power Query** – data preparation and transformation
- **DAX** – measures and KPI calculations
- **Data Modeling** – employee analytics model
- **Interactive Visualizations** – cards, slicer, line chart, pie chart, column chart, bar charts, and donut chart

---

## 📁 Dashboard Structure

The current Power BI report contains one main dashboard page with the following visuals:

| Visual | Purpose |
|---|---|
| Total Employees | Shows total workforce size |
| Employees in HQ | Shows percentage of employees working from headquarters |
| Remote Employees | Shows percentage of employees working remotely |
| Attrition Rate | Shows the reported employee attrition rate |
| Avg. Age | Shows average employee age |
| Rate of Hire by Year | Shows hiring distribution across years |
| Total Employees by Race | Shows workforce composition by race |
| Attrition by Department | Compares terminated employees across departments |
| Total Employees by Department | Shows workforce size by department |
| Active vs Terminated Employees | Shows employee-status composition |
| Employees by Job Title | Shows the distribution of employees across roles |
| Department Slicer | Allows users to filter the dashboard by department |

---

## 📌 Key KPIs in the Current Dashboard

The dashboard currently displays:

- **Total Employees:** 22K
- **Employees in HQ:** 75.2%
- **Remote Employees:** 24.8%
- **Attrition Rate:** 35%
- **Average Age:** 38

> KPI values are based on the current report view and can change when filters are applied.

---

## 🔍 Business Insights

### 1. Workforce Size

The dashboard reports approximately **22K employees**, providing the overall workforce scale used for the analysis.

### 2. HQ vs Remote Workforce

Approximately **75.2% of employees work in headquarters locations**, while **24.8% are remote employees**.

This provides HR teams with a useful starting point for evaluating workplace strategy, office capacity, and remote-work requirements.

### 3. Attrition

The dashboard reports an **attrition rate of 35%**.

This makes employee retention an important area for further investigation. The dashboard can be used to identify which departments have higher termination counts, but additional dimensions such as tenure, compensation, performance, and exit reason would be needed to determine root causes.

### 4. Department Workforce Concentration

Engineering is the largest department in the current dashboard view at approximately **6.7K employees**, followed by Accounting at approximately **3.3K**.

The remaining departments have considerably smaller workforce populations.

This distribution can support workforce planning, recruitment allocation, and department-level capacity analysis.

### 5. Department-Level Terminations

The **Attrition by Department** visual compares terminated employees across departments.

In the current dashboard view, **Sales displays 335 terminated employees**. The visual can be used interactively to compare termination counts across departments.

### 6. Hiring Distribution Over Time

The **Rate of Hire by Year** visual shows the percentage distribution of employee records by hire year.

This can help HR teams understand hiring concentration across historical periods and identify periods of stronger or weaker recruitment activity.

> Note: the current visual is configured as a percentage-of-total employee count by hire year. Therefore, it should be interpreted as the **share of employees hired in each year**, rather than a conventional annual hiring rate.

### 7. Workforce Composition by Race

The dashboard includes a race-distribution visualization. The largest visible category is **White at 28.49%**, followed by other reported categories such as Two or More Races, Black or African American, Asian, Hispanic or Latino, and American Indian or Alaska Native.

This visual can support workforce diversity reporting and demographic monitoring.

### 8. Active vs Terminated Employees

The donut chart shows the split between active and terminated employees.

The current dashboard displays approximately:

- **82.31% Active**
- **17.69% Terminated**

This percentage view should be interpreted separately from the dashboard's reported **35% Attrition Rate**, because the two metrics measure different concepts depending on their underlying definitions.

### 9. Job Title Distribution

The job-title chart highlights the roles with the largest employee populations.

The visible dashboard values include approximately:

- Research Assistant – 754
- Business Analyst – 708
- Human Resources – 613
- A research-related role – 538
- Account Executive – 505

This can support role-based workforce planning and recruitment analysis.

---

## 🚨 Business Problems Identified

### Problem 1 — Employee Retention

A reported attrition rate of 35% indicates that retention deserves closer analysis.

**Questions to investigate:**
- Which departments have the highest attrition?
- Is attrition higher among newer employees?
- Does compensation relate to attrition?
- Are particular job titles more affected?
- Are remote and HQ employees showing different patterns?
- What are the main exit reasons?

### Problem 2 — Workforce Concentration

A large share of employees is concentrated in Engineering and Accounting.

HR may need to monitor whether recruitment, training, succession planning, and workforce capacity are aligned with this concentration.

### Problem 3 — Workplace Location Strategy

With 75.2% of employees shown as HQ-based and 24.8% remote, HR can evaluate:

- Office capacity
- Remote-work policies
- Hybrid workforce requirements
- Location-specific hiring
- Employee productivity and retention by work location

### Problem 4 — Hiring Pattern Visibility

Historical hiring distribution is visible, but the dashboard does not currently explain **why** hiring increased or decreased in particular years.

Additional business context such as company growth, hiring plans, acquisitions, or economic conditions could improve interpretation.

### Problem 5 — Limited Root-Cause Analysis

The current dashboard identifies **what is happening**, but not all of the reasons **why it is happening**.

Useful additional attributes would include:

- Employee tenure
- Salary
- Performance rating
- Job level
- Promotion history
- Overtime
- Employee satisfaction
- Exit reason
- Recruitment source

---

## 💡 Recommended Future Enhancements

### HR Retention Analysis

Add:

- Attrition by tenure
- Attrition by salary band
- Attrition by job title
- Attrition by location
- Attrition by age group
- Attrition by gender
- Voluntary vs involuntary termination
- Exit-reason analysis

### Hiring Analysis

Add:

- Monthly/quarterly hiring trend
- New hires vs replacements
- Hiring by department
- Hiring by location
- Hiring source
- Recruitment funnel metrics

### Workforce Planning

Add:

- Headcount forecast
- Department capacity
- Open positions
- Employee-to-manager ratio
- Retirement/tenure risk
- Skills inventory

---

## 📂 Suggested GitHub Repository Structure

```text
HR-Analysis-PowerBI/
│
├── README.md
├── HR Analysis.pbix
│
├── docs/
│   └── HR_Analysis_Business_Insights_and_Problems.pdf
│
├── images/
│   └── HR_Analysis_Dashboard.png
│
└── data/
    └── README.md
```

If the original employee dataset is confidential or not yours to redistribute, do **not** upload it to GitHub. Keep the repository focused on the PBIX/report and documentation.

---

## 📈 Skills Demonstrated

This project demonstrates practical skills in:

- Data visualization
- Power BI dashboard development
- KPI design
- DAX measures
- Power Query
- Data modeling
- Slicers and interactive filtering
- HR analytics
- Workforce analysis
- Attrition analysis
- Business problem identification
- Business storytelling
- Dashboard UI/UX

---

## 🧠 Key Takeaway

The dashboard provides a high-level HR view by connecting **workforce size, location, attrition, hiring distribution, demographics, departments, employee status, and job titles** in a single interactive report.

The next analytical step is to move from descriptive reporting to **root-cause analysis and workforce planning** by adding tenure, compensation, performance, exit reasons, and other employee-level drivers.

---

## 👤 Author

**[Your Name]**

Data Analyst | Power BI | SQL | Python | Excel

