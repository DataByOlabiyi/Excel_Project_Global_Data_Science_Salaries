# Global Data Science Salaries During the COVID-19 Era: A Data Transformation and Analytics Dashboard

## Introduction

The COVID-19 pandemic placed the world in a very troubled scenario, leaving no industry unscathed — and data science was no exception. During this period, demand for data-driven roles increased massively as companies needed insights to navigate the uncertainty. That demand directly impacted salaries, influenced further by geography, experience level, and a massive jump in remote work.

This study uses a bifurcated methodology to track global data science salary trends during the pandemic:

### Quantitative Approach
- Compiles salary information for various regions, job titles, and experience levels.
- Conducts research on the effect of organizational scale and work-from-home arrangements on remuneration.

### Qualitative Approach
- Explores the challenges that organizations and individuals faced in adapting to new workforce dynamics.

By integrating these perspectives, this analysis gives an all-encompassing understanding of the evolution of data science salaries in this unmatched era of transformation.

## Problem Statement

The pandemic induced significant changes in the labor market, as many organizations transitioned to remote or hybrid work models. These changes impacted compensation structures in ways that are not easily visible through raw data. Key challenges include:

- **Inconsistent Data**: Currency differences, and abbreviations in records.
- **Incompatibility Problem**: Rewards denominated in local currencies without adjusting for exchange rate movements.
- **Regional Inequalities**: The economic impact of the pandemic varied across regions.

Through the transformation and analysis of this data, we aim to fill the gaps and provide actionable insights for enterprises, recruiters, and professionals.

## Data Overview

The dataset contains global salary data for data science jobs, collected during the COVID-19 era (2020–2022). It includes data on various aspects of compensation and work environments, such as:

- **work_year**: The year the data was recorded.
- **job_title**: The actual role title, for instance, Data Scientist or Machine Learning Engineer.
- **experience_level**: Categories such as Entry (EN), Mid (MI), Senior (SE), and Executive (EX).
- **employment_type**: Full-time (FT), Part-time (PT), Contract (CT), Freelance (FL).
- **Remuneration**: Earnings recorded in the relevant local currency.
- **salary_currency**: The currency in which the salary was paid.
- **remote_ratio**: Percentage of the job done remotely (0%, 50%, 100%).
- **company_location, employee_residence**: Geolocation data for the company and employee.
- **company_size**: Organization size — Small (S), Medium (M), and Large (L).

## Data Cleaning/Transformation

The data was cleaned and transformed to ensure consistency and comparability. Here is a step-by-step breakdown:

1. **Currency Exchange**
   - **Issue**: Compensation was recorded in various currencies.
   - **Solution**: Historical exchange rates (relevant to work_year) were applied to convert all salaries to USD, creating a new column, salary_USD.

2. **Normalizing Labels**
   - Abbreviations were expanded to improve readability, e.g., “SE” to “Senior,” “FT” to “Full-Time,” and “S” to “Small.”

3. **Geographic Insights**
   - Extracted country and region fields from employee_residence and company_location.
   - Mapped countries to regions (e.g., “Nigeria” → “Africa”).

4. **Role Categorization**
   - Grouped roles in job_title into broader categories:
     - Data Science (e.g., Data Scientist).
     - Machine Learning (e.g., Machine Learning Engineer).
     - Data Engineering (e.g., Data Engineer).

5. **Classifying Remote Work**
   - Converted remote_ratio to a descriptive category:
     - 0% → On-site
     - 50% → Hybrid
     - 100% → Remote

### Comparison of Raw vs. Clean Data

In the raw dataset, inconsistencies in salaries and missing values made comparisons unreliable. The cleaned dataset standardized these variables, making the analysis both accurate and fair.

## Data Analysis

The Global Data Science Salaries Dashboard was used to analyze big trends and visualize insights. Here are the findings:

1. **Sum of Salary (KPI)**
   - The total sum of salaries across all regions, roles, and experience levels amounts to $67,972,324.54. This significant figure highlights the growing investment in data professionals as companies leaned heavily on data-driven decisions during the COVID-19 era.

2. **Company Size by Average Salary (Pie Chart)**
   - **Large Companies**: Offering the highest average salary at $119,222, likely due to their robust resources and ability to attract top talent.
   - **Medium Companies**: Slightly lower average salary of $116,349, reflecting their competitive nature in compensation.
   - **Small Companies**: The lowest average salary of $77,547, indicating budget constraints yet potentially offering advantages like flexibility.

3. **Experience Level by Average Salary (Bar Chart)**
   - **Executive Roles**: Lead with an average salary of $199,196, underscoring the value of leadership and strategic expertise.
   - **Senior Professionals**: Earn an average salary of $138,478, reflecting their advanced experience.
   - **Mid-level Professionals**: Average $87,345, a midpoint in career progression.
   - **Entry-level Employees**: Start at $61,532, indicative of initial roles in the career ladder.

4. **Employment Type by Average Salary (Bar Chart)**
   - **Contract Roles**: Command the highest average salary of $184,290, likely due to specialized skills and short-term demand.
   - **Full-time Roles**: Offer a stable average salary of $113,147.
   - **Freelance Positions**: Average $48,000, reflecting variability and independence.
   - **Part-time Roles**: Earn the lowest average salary of $32,848, reflecting reduced hours and scope.

5. **Geographical Insights: Average Salary by Employee Region (Bar Chart)**
   - **North America**: Tops the list with $144,316, showcasing a strong market for talent.
   - **Oceania**: Follows with $112,130.
   - **Africa ($39,944)** and **Central America ($20,000)**: Record the lowest averages, indicating regional economic disparities.

6. **Average Salary by Remote Work Level (Bar Chart)**
   - **Fully Remote Jobs**: Lead with an average of $122,203, highlighting demand for flexibility and a global talent pool.
   - **On-site Roles**: Average $105,682, offering stable, traditional setups.
   - **Hybrid Roles**: Lowest at $80,723, possibly reflecting challenges in balancing remote and in-person responsibilities.

7. **Remote Work Level Distribution by Category (Line Chart)**
   - **Data Engineering and Machine Learning Roles**: Show consistently higher salaries, peaking in fully remote setups.
   - **On-site and Hybrid Roles**: Generally lower earnings, suggesting reduced demand compared to fully remote options during the pandemic.

8. **Trends by Experience Level (Line Chart)**
   - **Executive Salaries**: Peaked in 2021 at $223,675, highlighting increased leadership demand during the pandemic.
   - **Entry-level Salaries**: Grew steadily from $63,627 (2020) to $64,795 (2022).
   - The gap between Entry-level and Senior roles widened over time, emphasizing the importance of experience in driving higher compensation.

9. **Average Salary by Department (Bar Chart)**
   - **Leadership/Management Roles**: Report the highest average salaries, closely followed by Machine Learning and AI.
   - **Data Analysis Roles**: Average the lowest salaries, likely reflecting a less specialized skill set.

10. **Yearly Average Salary (Line Chart)**
    - Salaries increased from $95,817 (2020) to $123,885 (2022), driven by the growing demand for data professionals and the rise of remote opportunities during the pandemic.

11. **Global Average Salary (Choropleth Map)**
    - **North America and Oceania**: Dominate in compensation.
    - **Africa and Central America**: Display significant pay gaps, reflecting regional economic differences.

12. **Average Salary by Company Size (Bar Chart)**
    - **Large Companies**: Lead with $119,222, reflecting their capacity to offer competitive pay.
    - **Medium Companies**: Close behind at $116,349, showing strong competitiveness.
    - **Small Companies**: Lag at $77,547, potentially offset by flexibility or niche opportunities.

## Key Takeaways

### Geographic Pay Differences
- Salaries varied greatly across regions due to differences in economic development, cost of living, and demand for data professionals.
- North America and Oceania offered higher remuneration, whereas Africa and Central America exhibited lower salary levels.

### Pandemic’s Impact on Remote Work
- Remote work significantly altered compensation structures, with fully remote positions offering higher pay.
- Remote flexibility became a major driver of employee satisfaction and productivity.

### Role-Based Trends
- Specialized roles, such as Machine Learning Engineers, commanded higher salaries due to their critical contributions to AI-driven innovation.

### Company Size and Compensation
- Larger organizations offered higher average salaries, while smaller organizations presented opportunities for higher remuneration in niche environments.

### Experience Matters
- Salaries rose with experience, with exponential increases for Senior and Executive roles.

### Yearly Growth and Pandemic Effect
- Data science salaries remained resilient and showed consistent growth during the pandemic, highlighting the critical role of data professionals in crisis management.

## Overview Dashboard

This interactive dashboard allows users to explore:
- Salary trends by region, role, and experience level.
- The impact of remote work on wages.
- Disparities by organizational scale and employment type.

### Key Ingredients
- **Filter Pane**: Narrow down analysis by years, roles, and regions.
- **Summarized Metrics**: High-level KPIs for quick insights.
- **Visualizations**: Charts and graphs to highlight key trends.

## Conclusion

The COVID-19 era reshaped the global data science landscape, presenting both challenges and opportunities. This dataset and dashboard empower professionals and organizations to navigate salary trends, ensuring fairness and competitiveness in compensation.

To see the full analysis in action, check out the dashboard — screenshots and links are provided.
