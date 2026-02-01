# US Health Insurance Analytics Dashboard

![Insurance dashboard](https://github.com/visakhjp/US-Health-Insurance-analytics/blob/main/US%20Health%20Insurance%20analytics%201.JPG)
![Insurance dashboard](https://github.com/visakhjp/US-Health-Insurance-analytics/blob/main/US%20Health%20Insurance%20analytics%202.JPG)
![Insurance dashboard](https://github.com/visakhjp/US-Health-Insurance-analytics/blob/main/US%20Health%20Insurance%20analytics%203.JPG)

This interactive **Power BI dashboard** provides a comprehensive overview of US health insurance data, focusing on patient profiles, insurance charges, and the main risk drivers: **BMI**, **smoking status**, **age**, and **region**.

## Objective

Deliver clear, actionable insights into the factors that drive higher insurance costs.  
Helps insurance providers, analysts, and stakeholders quickly identify:

- Trends and patterns in medical charges
- High-risk patient profiles
- Demographic and geographic cost variations

## Dataset

- **Name**: US Health Insurance Dataset (commonly known as Medical Cost Personal Datasets)
- **Source**: https://github.com/visakhjp/US-Health-Insurance-analytics/blob/main/Insurance-USA.xlsx
- **Rows**: 1,338 insured individuals
- **Columns**: age, sex, bmi, children, smoker, region, charges

## Key Performance Indicators (KPIs)

 KPI                                                     
 Total Charges - Cumulative insurance costs               
 Average Charges - Mean cost per patient                    
 Number of Applicants - Total patients in dataset                
 Average BMI - Mean Body Mass Index                     
 Average Children - Mean number of dependents                

## Project Process

1. **Data Acquisition**  
   Downloaded patient records (age, sex, BMI, children, smoker, region, charges)

2. **Data Cleaning**  
   - Standardized categorical values (e.g. smoker: "yes"/"no")  
   - Checked and handled missing values (dataset is clean)

3. **Feature Engineering**  
   - Created **Age Bins**: 18-24, 25-34, 35-44, 45-54, 55-64  
   - Created **BMI Categories**: Underweight, Normal, Overweight, Obese

4. **DAX Calculations**  
   - Average / Total Charges  
   - Average BMI & Children  
   - **Top 10% Flag** - identifies the most expensive 10% of patients

5. **Visualizations**  
   - **Cards** - main KPIs  
   - **US Region Map** - patient count & avg charges by region  
   - Bar/Column charts - charges by smoker status, age group  
   - Scatter plot - BMI vs Charges (with trend line)  
   - Treemap - charges by BMI category  
   - Funnel chart - charges by number of children  
   - Additional visuals for top 10% costly patients

6. **Interactivity & Design**  
   - Slicers: Gender, Region, Smoker, Age Bin  
   - Consistent professional theme (blue + white)  
   - Three pages: **Patient Analysis**, **Cost Analysis**, **Risk Analysis**

7. **Validation & Publishing**  
   - Cross-checked calculations and filters  
   - Published to Power BI Service

## Dashboard Pages

- **Patient Analysis**  
  Explore demographics, regional distribution, age & BMI profiles

- **Cost Analysis**  
  Understand how smoking, obesity, age and children drive premiums

- **Risk Analysis**  
  Deep dive into characteristics of the **top 10% most expensive** applicants

## Key Insights

- **Smoking** is the strongest cost driver  
  Smokers: ~$32,000 avg | Non-smokers: ~$8,000 avg (**4× higher**)

- **BMI** shows strong positive correlation with charges  
  **Obese** category has the highest average charges (~$15,550)

- **Regional** pattern  
  Southeast has the largest number of applicants  
  Slightly elevated charges in some regions

- Costs increase significantly with age, peaking in the **50–64** bin

- **Top 10%** most expensive patients are **almost exclusively** smokers with high BMI

## Conclusion & Business Recommendations

Lifestyle factors - particularly **smoking** and **high BMI** - are the dominant drivers of insurance costs.

**Potential actions for insurers / health organizations:**

- Invest in **smoking cessation** programs
- Promote **weight management** and wellness initiatives
- Adjust premium pricing models to better reflect age-related risk
- Pay special attention to health trends in high-density regions (e.g. Southeast)

## Technologies Used

- **Power BI Desktop** - data modeling, DAX, visuals  
- **Excel** Initial EDA and data validation
- **DAX** for measures & flags


Feel free to contribute, fork, or use this project as inspiration!

If you find this dashboard useful, give the repo a star!
