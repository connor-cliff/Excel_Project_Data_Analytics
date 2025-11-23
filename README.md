# Data Jobs Analysis Project (Excel)

This Excel project was created with the aim to analyse the data science job market and understand what employers are looking for while providing a great oppertunity to to practise advanced Excel skills.

## Objectives
The analysis focuses on four questions:
1. Do job postings that list more skills tend to offer higher salaries?
2. How do salaries differ by region?
3. What are the most common skills in data roles?
4. What are the top-paying skills?

## Excel Skills Practised
- Power Query (ETL)
- Power Pivot and Data Model  
- PivotTables  
- PivotCharts  
- Basic DAX measures

## Power Query (ETL)
Two queries were created and cleaned:
- **Jobs table**: job information  
- **Skills table**: individual skills linked by job ID  

Each query was transformed by changing column types, removing unnecessary columns, cleaning text to eliminate specific words, and trimming excess whitespace.

### data_jobs_all
<img src="Resources/salary_transform.JPG">

### data_jobs_skills
<img src="Resources/skills_transform.JPG">

Each query was then loaded into the workbook to be used for subsequent analysis.

### data_jobs_all
<img src="Resources/salary_load.JPG">

### data_jobs_skills
<img src="Resources/skills_load.JPG">

## Power Pivot & DAX
A relationship was created between the jobs and skills tables using the **job_id** field.

<img src="Resources/data_model.JPG">

## Key Analysis

### 1. Skills vs Salary
Counted the number of skills per job and compared this with median salary using PivotTables.

<img src="Resources/skills_money.JPG">

### 2. Salary by Region
Created DAX measures to calculate median salary. Example:

Median Salary :=
MEDIAN(data_jobs_all[salary_year_avg])


> **Add screenshot here** – DAX measure  
<img src="Resources/data_model.JPG">

### 3. Most Common Skills
Aggregated skill frequency using the data model to identify the most frequently listed skills.

<img src="Resources/skill_analysis.JPG">

### 4. Top-Paying Skills
Built a combo PivotChart to compare median salary with how often each skill appears.

<img src="Resources/top_skills.JPG">

## Files
- `Data_Jobs_Analysis.xlsx` – workbook with queries, model, PivotTables, and visuals.


