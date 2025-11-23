# Data Jobs Analysis Project (Excel)

This Excel project was created with the aim to analyse the data science job market and understand what employers are looking for while providing a great oppertunity to to practise advanced Excel skills.

## Objectives
The analysis focuses on four questions:
1. Do job postings that list more skills tend to offer higher salaries?
2. How do salaries differ by region?
3. What are the most common skills in data roles?
4. What are the top-paying skills?

## Excel Skills Practised
- Power Query  
- Power Pivot and Data Model  
- PivotTables  
- PivotCharts  
- Basic DAX measures

## Data Preparation (Power Query)
Two queries were created and cleaned:
- **Jobs table**: job information  
- **Skills table**: individual skills linked by job ID  

Steps included changing data types, removing unnecessary columns, and standardising text.

> **Add screenshot here** – Power Query setup

## Data Model (Power Pivot)
A relationship was created between the jobs and skills tables using the **job_id** field.

> **Add screenshot here** – Data Model diagram

## Key Analysis

### 1. Skills vs Salary
Counted the number of skills per job and compared this with median salary using PivotTables.

> **Add chart screenshot here**

### 2. Salary by Region
Created DAX measures to calculate median salary. Example:

