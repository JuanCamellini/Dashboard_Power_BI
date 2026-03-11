# 📊 Argentina Data Jobs Dashboard

## 📌 Project Overview

This project analyzes the **Data Job market in Argentina** using an interactive dashboard built in **Power BI**.

The goal of this project is to transform raw job posting data into **clear visual insights about the data industry**, helping identify:

- the most **in-demand technical skills**
- the **highest paying roles**
- salary distribution across different data positions

Users can explore the data dynamically through **interactive filters and parameter-based visuals**, enabling flexible analysis of the job market.

## 📦 Dataset

The dataset used in this project contains job postings collected from multiple online job platforms.

Dataset characteristics:

- Format: CSV
- Size: Over **2.4 million records**
- Content: Job postings related to data and technology roles
- Includes information such as:
  - job title
  - required skills
  - salary information
  - job location
  - company data

The dataset was processed and transformed using **Power Query** before being modeled inside Power BI.

---

## 🧠 Business Questions

This dashboard was designed to answer key questions about the data job market:

- What are the **most demanded skills** in data-related jobs?
- Which **roles offer the highest salaries** in the data industry?
- How many **skills are typically required per job posting**?
- What is the **median salary for different data roles**?
- How does job demand change depending on the **selected role or location**?

The goal is to help understand the **current demand for technical skills and salary trends** in the data industry.

---

## 🖥️ Dashboard Preview

![Dashboard](/Argentina_data_jobs\images\Argentina_data_jobs_dashboard.png)

---

## ⚙️ Dashboard Features

The report includes several interactive elements designed to enhance data exploration.

- 📌 **KPI Cards**
  - Total Job Count
  - Skills Per Job
  - Median Monthly Salary
  - Median Hourly Salary

- 🎛️ **Dynamic Filtering**
  - Country slicer
  - Job Title slicer
  - Clear slicers button for quick reset

- 🔄 **Field Parameters**
  - Allows switching the **X-axis metric dynamically** in charts
  - Enables comparison between different analytical perspectives

- 📊 **Interactive Visualizations**
  - Top Demanded Skills
  - Top Paying Data Jobs

---

## 🗂️ Data Model

The project uses a relational data model connecting job postings with related attributes such as skills and job titles.

This structure allows efficient filtering and aggregation across the dashboard.

![Data Model](/Argentina_data_jobs/images/Model_View.png)

---

## 📊 DAX Measures

Below are some of the key DAX measures used in the dashboard.

### Grand Total Skill Count

```DAX
Grand Total Skill Count = 
CALCULATE(
    SUM(job_postings_fact[skill_count]),
    ALL(job_postings_fact)
)
```

This measure calculates the **total number of skills requested across all job postings**, ignoring any filters applied to the dataset.

---

### Monthly Median Salary

```DAX
Monthly Median Salary = 
DIVIDE(
    MEDIAN(job_postings_fact[salary_year_avg]),
    12
)
```

This measure converts the **median yearly salary into a monthly salary estimate**.

---

### Median Hourly Salary

```DAX
Median Hourly Salary = 
MEDIAN(job_postings_fact[salary_hour_avg])
```

This measure calculates the **median hourly salary across job postings**.

---

### Job Percentage

```DAX
Job Percentage = 
DIVIDE(
    [Job Count],
    CALCULATE(
        [Job Count],
        ALLSELECTED(skills_dim)
    )
)
```

---

## 🛠️ Tools & Technologies

- 📊 Power BI
- 🔄 Power Query
- 🧮 DAX
- 📈 Field Parameters
- 🗄️ Data Modeling

---

## 🔎 Key Insights

The dashboard allows several insights about the Argentine data job market:

- 🐍 **Python and SQL** are the most demanded skills in data-related roles
- ☁️ Cloud technologies such as **AWS and Azure** are frequently requested
- 💰 Roles like **Cloud Engineer** and **Software Engineer** show the highest median salaries
- 🧠 Data jobs typically require **multiple technical skills per posting**

---

## 🎯 Project Purpose

This project was created as part of my **Data Analytics portfolio** to demonstrate practical skills in:

- data visualization
- business intelligence reporting
- data modeling
- interactive dashboard development

---

## 👨‍💻 Author

Juan Camellini

Aspiring **Data Analyst** focused on:

- Python
- SQL
- Power BI
- Data Visualization
- Business Intelligence