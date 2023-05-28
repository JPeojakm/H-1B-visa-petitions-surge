# H-1B-visa-petitions-surge

H-1B visa lottery system
Data Reporter: Jinpeng Li, jinpeng.business@gmail.com

Each year, U.S. Citizenship and Immigration Services grants 65,000 new H-1B visas to applicants with bachelor's or higher degrees, and an additional 20,000 visas to those with master's or higher degrees. However, due to the high number of sponsorship applications, USCIS uses a lottery system to ensure the number of visas remains within the quota and determine which applications to review.

This project is for Professor Christian McDonald's Spring 2023 section of Reporting with Data. I will utilize the data sets from the Department of Labor and USCIS to analyze H1B visa applicants from the past five years, with a focus on two key aspects: Cities and Occupations. The following questions will be addressed:

1. What is the trend of H1B sponsorship in Texas? This involves determining the number of petitions Texas has applied for in the past five years and calculating the approval rate.
2. Which state submits the highest number of H1B visa applications?
3. What types of positions do U.S. employers prefer to sponsor for H1B visas? The analysis will cover two industries: computer science and journalism.
4. What is the average salary of H1B applicants in each state?
5. Which company submits the most petitions?

To present the findings, I will use Datawrapper to create line charts depicting the demand for H-1B visas, specifically highlighting the recent surge in application numbers due to fraud. Additionally, a stacked chart will be created to illustrate the distribution of occupations. For displaying the quantity of H-1B visa applicants in different cities, I will utilize d3 and mapbox to generate a map. The analysis will reveal that Texas and the Bay Area have the highest number of H-1B petitions.

## Data Overview:

The raw data was obtained from the Department of Labor (DoL) and U.S. Citizenship and Immigration Services (USCIS). There are two main types of CSV files included in the dataset. The first type is the "LCA_FY_year" file, which contains information on petitions. The second type is the "h1b_datahubexport-year" file, which includes data on applicants who have been granted H-1B visa eligibility.

The DoL Spreadsheet includes the following fields: 
- Visa class
- Employer name
- SOC title
- Job title
- City
- State
- Prevailing wage
- Employer location

Using the available information, I utilized the tidyverse package to filter the H-1B visa petitions and clean up the City and State columns for further analysis.
