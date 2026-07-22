# 📊 HR Analytics Power BI Dashboard

An interactive, enterprise-style Human Resources analytics dashboard built in Power BI, delivering real-time workforce intelligence across Attrition, Compensation, and Performance — supported by a fully custom HTML/CSS-driven UI layer.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Data%20Modeling-blue?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-orange?style=for-the-badge)
![HTML/CSS](https://img.shields.io/badge/HTML%2FCSS-Custom%20Visuals-purple?style=for-the-badge&logo=html5)

---

## 🎯 Business Problem

HR teams often struggle to answer strategic workforce questions in real time: *Why are we losing people? Is our pay structure equitable? Are managers driving engagement or burnout?*

This dashboard consolidates 311 employee records into a single source of truth, replacing static spreadsheet reporting with an interactive, drill-down analytics hub that surfaces attrition drivers, compensation equity, and performance trends at a glance.

---

## 🖼️ Dashboard Preview

### 🏠 Home — Landing Hub
Interactive navigation hub with a custom-designed HTML/CSS welcome screen and quick access to all report pages.

![Home](images/01-home.png)

### 👥 Attrition & Retention
Tracks historical turnover (2010–2018), termination reasons, and department-level attrition rates.

**Key Insights:**
- Overall attrition rate: **33.44%** | Voluntary turnover: **28.30%**
- Highest attrition by department: **Production (39.7%)** and **Software Engineering (36.4%)**
- Top termination drivers: another position, general dissatisfaction, compensation

![Attrition](images/02-attrition.png)

### 💰 Compensation
Analyzes pay distribution across gender, age groups, and performance tiers to surface equity gaps.

**Key Insights:**
- Average salary: **$69,021** | Range: $45,046 – $250,000
- Gender pay gap: **4.02%** (moderate)
- Top performers ("Exceeds") earn noticeably more on average than "PIP" tier employees

![Compensation](images/03-compensation.png)

### 📈 Performance
Monitors engagement, absenteeism, and performance distribution across managers and departments.

**Key Insights:**
- 78.1% of employees fall in the "Fully Meets" performance tier
- PIP rate: **4.18%** | Average satisfaction score: **3.9 / 5**
- Highest engagement scores reported under Board of Directors and senior leadership

![Performance](images/04-performance.png)

---

## 🧩 Data Model

Built on a clean **Star Schema** for optimal DAX performance and scalability:

- `Fact_Employees` — core employee-level transactional data
- `Dim_Department`
- `Dim_Manager`
- `Dim_Position`
- `Dim_RecruitmentSource`
- `Dim_PerformanceRating`

Relationships are modeled 1-to-many from dimension to fact tables, enabling cross-filtering across all report pages via slicers (Department, Manager, Position, Recruitment Source, Gender).

---

## 🛠️ Tools & Techniques

| Category | Details |
|---|---|
| **Data Modeling** | Star Schema, relationship optimization, calculated tables |
| **DAX** | KPI measures, YoY trends, rate/ratio calculations, dynamic titles |
| **Power Query** | Data cleaning, type transformation, conditional columns |
| **Custom Visuals** | Hand-coded HTML/CSS KPI cards, animated welcome screen, gradient dividers |
| **UX Design** | Dark-themed enterprise UI, consistent sidebar navigation, responsive KPI layout |

---

## 📌 Key Metrics at a Glance

| Metric | Value |
|---|---|
| Total Employees | 311 |
| Active Employees | 207 |
| Attrition Rate | 33.44% |
| Average Salary | $69,021 |
| Gender Pay Gap | 4.02% |
| PIP Rate | 4.18% |
| Avg. Satisfaction Score | 3.9 / 5 |

---

## 🚀 How to Use

1. Clone this repository
2. Open `HR_Dashboard.pbix` in Power BI Desktop
3. Refresh the data source connection if prompted
4. Explore each page (Home, Attrition, Compensation, Performance) using the left navigation panel and slicers

---

## 📬 Connect With Me

**Belal Farrag** — Data Analyst | Power BI Developer
🔗 [LinkedIn](https://linkedin.com/in/belal-farrag-b976b01a4/)
🔗 [GitHub](https://github.com/belalfarrag95)

---

*Built with Power BI, DAX, and a lot of custom CSS ✨*
