 ## COVID-19 Impact on Sri Lanka’s Tourism Industry ##

## Project Overview ##
This project analyzes the impact of the COVID-19 pandemic on Sri Lanka’s tourism industry using an interactive Power BI dashboard. The analysis focuses on tourist arrivals, tourism revenue, year-over-year (YOY) growth trends, recovery patterns, and changes in global tourist source countries across different COVID-19 phases.The dashboard provides insights into how tourism was affected before COVID-19, during the pandemic, and in the post-COVID recovery period.

## Objectives ##
- Analyze monthly and yearly tourist arrival trends
- Measure tourism revenue performance across COVID periods
- Identify worst-impact and best-recovery months
- Evaluate YOY growth in arrivals and revenue
- Visualize top tourist source countries globally
- Compare tourism performance before, during, and after COVID-19

  ## Dataset ##
- Toursim Arrivals Dataset : https://www.sltda.gov.lk/en/statistics (8 separate Datasets from SLTDA from 2018- 2025)
- Toursim Revenue : https://tradingeconomics.com/sri-lanka/tourism-revenues (2018-2025)
  
## Tools & Technologies ##
- Power BI Desktop
- SQL Query (Data Cleaning & Transformation)
- DAX (Data Analysis Expressions)
- Power Query(Data Cleaning & Transformation)
- Data Modeling(Star Schema with Date Table)
  
## Methodology ##
## Data Collection ##

Tourism-related data (Toursim-Arrivalls and Toursim-Revenue) was collected covering the period from 2018 to 2025, including:

- Data Cleaning & Preparation
- Data preparation was performed using SQL Query and Power Query, including:
  - Handling missing values and missng rows
  - Created a singel dataset for Toursim arrival by combining 8 datasets using UNION ALL
  - Standardizing country names to ensure uniqueness and consistency
  - Removing invalid, ambiguous, or incomplete country records
  - Creating a unified YearMonth field for time-based analysis
  - Ensuring correct data types for numeric and date-related columns

## Data Modeling ##
A proper data model was created using a star schema approach:
- Fact Table:Tourist arrivals and revenue data
- Date Table: Custom date table created using Year and Month fields
- Advanced DAX measures were created to enable time intelligence and performance analysis
  
## Key modeling steps ##:
- Established relationships between fact and date tables
- Created a COVID period classification (Before-COVID, During COVID, Post-COVID)
- Avoided circular dependencies by separating calculated columns and measures

 ## Dashboard Features ##
 ## KPI Indicators ##
- Total Tourist Arrivals
- Total Tourism Revenue
- Best Recovery Month (Post-COVID)
- First Worst COVID Month
  
## Advanced Visuals ##
- YOY Growth Trend Line Chart (Arrivals % & Revenue %)
- Monthly Arrivals Matrix by Year
- Tourist Arrivals & Revenue Over Time
- Tourism Revenue Breakdown by COVID Period and Year
- Top 10 Tourist Source Countries Map
  
## Interactive Filters ##
- Country
- Year
- Month
- COVID Period (Before, During, Post)
  
 ## COVID Period Classification ##
- Before-COVID: Up to December 2019
- During COVID: January 2020 – December 2021
- Post-COVID: January 2022 onwards This classification enables clear comparative analysis across pandemic phases.

 ## Key Insights
- Sharp decline in tourist arrivals during early 2020
- April 2020 identified as the first worst COVID month
- Strong recovery observed in early 2025
- YOY growth highlights rapid post-COVID rebound
- Shifts in top tourist source countries across periods

## Future Enhancements ##
- Forecasting tourism recovery using time-series models
- Regional clustering of tourist source countries
- Deeper country-level contribution analysis
- Integration with external economic indicators

## Author ##
Shayni Ravishika
Data Analytics & Business Intelligence Enthusiast
