# 🌎 Global Data Jobs Analytics Dashboard

## 📌 Project Overview

This project analyzes the **global data job market** using an interactive **Power BI dashboard with Drill Through functionality**.

The dashboard explores job demand, salary distribution, job platforms, and working conditions across different data-related roles worldwide.

A key feature of this report is the **Drill Through page**, which allows users to explore deeper insights for a selected job title, including salary statistics, remote work availability, education requirements, and job distribution across the world.

---

## 🧠 Business Questions

This dashboard was designed to answer several key questions about the global data job market:

- Which **data roles are most in demand worldwide**?
- What are the **average salaries for different data-related roles**?
- Which **platforms generate the most job postings**?
- What percentage of jobs offer **remote work**?
- How common is a **university degree requirement**?
- How are **data jobs geographically distributed** across the world?
- How many **technical skills are typically required per job posting**?

---

## 🖥️ Dashboard Preview

### Main Dashboard

![Dashboard](/Data_Jobs/images/Panel_Trabajo_Datos.png)

### Drill Through Page

![Drill Through](/Data_Jobs/images/Drill_Through.png)

---

## ⚙️ Dashboard Features

The report includes multiple interactive components to explore the dataset.

- 📊 **KPI Cards**
  - Total Job Count
  - Average Skills per Job
  - Average Annual Salary
  - Average Hourly Salary

- 🎛️ **Job Title Slicer**
  - Allows filtering all visuals by specific job roles

- 🔎 **Drill Through Analysis**
  - Users can select a job title and navigate to a **detailed analysis page**

- 📈 **Interactive Visualizations**
  - Job Count by Role
  - Job Trend Over Time
  - Job Platforms Distribution
  - Work Modalities

- 🌍 **Geographical Analysis**
  - Global map showing job distribution across different regions

---

## 🔍 Drill Through Analysis

The Drill Through page provides **detailed insights for a selected job title**.

When a user selects a job title and activates the Drill Through option, the report displays:

- 💰 Annual salary statistics
- ⏱️ Hourly salary statistics
- 🌐 Percentage of remote jobs
- 🎓 Percentage of jobs without university degree requirement
- 🏥 Percentage of jobs offering benefits
- 🌎 Global distribution of jobs for the selected role

This functionality allows deeper exploration of each role within the data job market.

---

## 🗂️ Data Model

The dataset was originally structured as a **flat table** containing job posting information.

To enable deeper analysis, a separate **skills table** was created and referenced in the model in order to calculate:

- number of skills required per job
- skill distribution across job postings

This approach allows more accurate aggregation and calculation of **skills per job metrics**.

![Model View](/Data_Jobs/images/Model_view.png)

---

## 📦 Dataset

The dataset used in this project contains job postings collected from multiple job platforms around the world.

Dataset characteristics:

- Format: CSV
- Size: Over **484.840**
- Source: Aggregated job posting dataset
- Includes information such as:
  - job title
  - salary data
  - job platform
  - job location
  - work modality
  - list skills

The dataset was processed and transformed using **Power Query** before being modeled in Power BI.

---

## 🛠️ Tools & Technologies

- 📊 Power BI
- 🔄 Power Query
- 🧮 DAX
- 📈 Drill Through
- 🗄️ Data Modeling
- 🌍 Geospatial Visualization

---

## 🎯 Project Purpose

This project is part of my **Data Analytics portfolio** and demonstrates practical skills in:

- interactive dashboard development
- business intelligence reporting
- drill-through analytics
- data modeling
- global labor market analysis

---

## 👨‍💻 Author

Juan Camellini

Aspiring **Data Analyst** focused on:

- Python
- SQL
- Power BI
- Data Visualization
- Business Intelligence