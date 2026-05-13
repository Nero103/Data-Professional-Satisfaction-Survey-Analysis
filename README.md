# Data Professional Satisfaction Survey Analysis

<img width="1434" height="806" alt="Data Professional Satisfaction Survey Overview" src="https://github.com/user-attachments/assets/5193d7bc-e501-4a1e-9770-f990305cfa9c" />

## Overview

This project analyzes real 2022 survey data from data professionals to better understand salary trends, career difficulty, job satisfaction, work/life balance, and programming language preferences across different countries and job titles.

The dashboard was built in Power BI and focuses on turning survey responses into clear, interactive business insights. The report includes an overall view as well as country-level views for the United States, Canada, India, United Kingdom, and Other regions.

## Project Goals

* Analyze compensation trends across data-related job titles
* Compare salary satisfaction and work/life balance satisfaction
* Identify which programming languages are most common by job role
* Understand how difficult respondents found it to enter the data profession
* Compare results across countries and regions
* Present findings through a clean, interactive Power BI dashboard

## Tools Used

* Power BI
* Power Query
* DAX
* Excel / CSV data preparation

## Dataset

The primary data source was survey response data from data professionals. The dataset included respondent-level fields such as but not limited to:

* Country
* Job title
* Age
* Average salary
* Salary satisfaction
* Work/life balance satisfaction
* Difficulty entering the data field
* Favorite programming language

## Dashboard Preview

### Overall Survey Dashboard

<img width="1434" height="806" alt="Data Professional Satisfaction Survey Overview" src="https://github.com/user-attachments/assets/88f79186-7c32-4dfa-960a-8ac7c71b9d07" />

The overall dashboard summarizes the full survey population, including total participants, average age, overall average salary, salary satisfaction, work/life satisfaction, job title salary comparisons, and programming language preferences.

## Country-Level Views

### United States

<img width="1439" height="808" alt="Data Professional Satisfaction Survey US" src="https://github.com/user-attachments/assets/25f6222c-d871-4d0c-8f98-7ad38696ab5b" />

The United States reported the highest overall average salary, with Data Scientists earning the highest average salary among job titles.

### Canada

<img width="1440" height="801" alt="Data Professional Satisfaction Survey Canada" src="https://github.com/user-attachments/assets/92ab1b79-e788-4bcb-ab7f-eb12526dfbfe" />

Canada showed strong salary performance overall, with higher average salaries than most regions outside the United States.

### India

<img width="1434" height="801" alt="Data Professional Satisfaction Survey India" src="https://github.com/user-attachments/assets/d3d59550-e7de-446f-b680-85bc383a65ca" />

India showed lower overall salary averages, but Data Scientists and Data Engineers still reported stronger compensation compared to other roles in the region.

### United Kingdom

<img width="1436" height="806" alt="Data Professional Satisfaction Survey UK" src="https://github.com/user-attachments/assets/8d89e909-fc9c-47f8-9c1b-036624aa159d" />

The United Kingdom showed moderate salary levels, with work/life balance satisfaction remaining higher than salary satisfaction.

### Other Regions

<img width="1430" height="801" alt="Data Professional Satisfaction Survey Other Regions" src="https://github.com/user-attachments/assets/8cb26fb7-21fe-4232-a152-939fc19069fb" />

The Other region category had lower average salaries overall, while still following the broader pattern of Data Scientists earning more than most other roles.

## Key Insights

* Most respondents reported that becoming a data professional was moderately difficult.
* Data Scientists earned the highest average salary overall at approximately $94K.
* The United States reported the highest salaries across nearly all data professions.
* Python was the most popular programming language across job titles.
* Salary satisfaction was lower than work/life balance satisfaction, suggesting compensation may be a weaker satisfaction driver than flexibility or work environment.
* Student and entry-level respondents reported the lowest average salaries across regions.

## Core DAX Measures

### Total Participants

```DAX
Total Participants =
DISTINCTCOUNT(SurveyData[Unique ID])
```
### Average Salary

```DAX
Overall Avg Salary =
AVERAGE(SurveyData[Average Salary])
```
### Average Salary Satisfaction

```DAX
Avg Salary Satisfaction =
AVERAGE(SurveyData[Q6 - How Happy are you in your Current Position with the following? (Salary)])
```
### Average Work/Life Satisfaction

```DAX
Avg WorkLife Satisfaction =
AVERAGE(SurveyData[Q6 - How Happy are you in your Current Position with the following? (Work/Life Balance)])
```
## Data Cleaning & Preparation

Before building the dashboard, the data was reviewed and prepared in Power Query. Key cleaning steps included:

* Reviewing column names and survey response fields
* Checking data types for numeric and categorical fields
* Cleaning salary values for analysis
* Preparing country and job title fields for filtering
* Creating measures for participant count, average salary, salary satisfaction, and work/life satisfaction
* Formatting salary values in thousands for readability

## Visualizations Included

* KPI cards for total participants, average age, average salary, salary satisfaction, and work/life satisfaction
* Country slicer buttons for interactive filtering
* Bar chart showing difficulty entering the data profession
* Bar chart showing average salary by job title
* Matrix heatmap showing salary by job title and country
* Treemap showing salary satisfaction by job title
* 100% stacked bar chart showing programming language preference by job title
* Key insights panel summarizing major findings

## Conclusion

This project demonstrates how survey data can be transformed into an interactive Power BI report that highlights compensation, satisfaction, and career trends across the data profession. The analysis shows clear differences across job titles and regions, with salary, satisfaction, and programming language preferences varying meaningfully by respondent group.
