# Forbes-Billionaires-Analysis
Exploring a bunch of information about really Rich people from Forbes


## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Findings](#findings)

### Project Overview
---
Motivated by a fascination for understanding wealth dynamics, this project uncovers captivating insights into the lives of the world's wealthiest individuals. 
From dissecting wealth distribution to revealing industry trends, this exploration navigates through data challenges to present a captivating visualization of the billionaire landscape.

### Data Sources
---
The primary source of information about the world's billionaires, published annually by Forbes magazine was gotten from [Kaggle](kaagle.com).

### Tools
---
- MySQL
  - Data Cleaning
  - Data Analysis
- PowerBI
  - Creating Visuals

### Data Cleaning
---
In the initial data preparation phase, I performed the following tasks:
1. Data loading and inspection.
2. Handling missing values.
3. Data Cleaning and Formatting.

### Exploratory Data Analysis
---

EDA involved exploring the forbes-billionaires-data to answer key questions, such as:
- What is the distribution of net worth among billionaires?
- What are the primary sources of wealth among billionaires?
- What proportion of billionaires are self-made versus those who inherited their wealth?
- How does the number of billionaires vary across different countries or regions?
- Which industries have the highest concentration of billionaires?
- How does marital status correlate with net worth?

### Data Analysis
---
I began exploring a bunch of information about really rich people from Forbes. I wanted to understand how these rich folks got their money and where they're from.
Did some Data Cleaning and Preprocessing.
Performed EDA to explore relationships between variables, distributions, and trends in the data.
Used SQL queries to generate descriptive statistics, histograms, box plots, and other visualizations to understand the data's characteristics.
```sql
--  top industries by the total net worth of billionaires involved in each industry?
SELECT industry, SUM(`net_worth`) AS total_net_worth
FROM forbes_billionaires
GROUP BY industry
ORDER BY total_net_worth DESC;

-- How many billionaires have completed a master's degree or a doctorate?
SELECT COUNT(*) AS count_of_billionaires
FROM forbes_billionaires
WHERE Master = 1 OR Doctorate = 1;
```
Interpreted the results of my analysis through reports and dashboards using Power BI.

![Forbes Billionaires Dashboard](https://github.com/chyonu/Forbes-Billionaires-Analysis/assets/91281098/9eea17f8-5175-46de-9106-529627092abe)

![forbes billionaires2_page-0002](https://github.com/chyonu/Forbes-Billionaires-Analysis/assets/91281098/ed0f05f2-a95d-4146-b390-faa4b33b98f3)


### Findings
---

The analysis findings are summarized as follows:
- The analysis revealed that Bernard Arnault & Family are the richest with a networth of two hundred and eleven billion dollars.
- The main sources of wealth among billionaires predominantly stem from diverse industries such as real estates, investments, diversified, and software.
  These industries contribute significantly to billionaires' amassed fortunes.
- A considerable portion of billionaires have self-made wealth, earned through entrepreneurship, business ventures, or innovation.
  However, a notable proportion also inherited their wealth from family or ancestors.
- The number of billionaires varies significantly across different countries or regions.
  Certain regions, such as North America and Asia, tend to have a higher concentration of billionaires compared to others.
- Industries like technology, real estate, telecom and sports boast a substantial concentration of billionaires.
  These sectors have contributed significantly to creating billionaire fortunes.

  [Learn more](https://app.powerbi.com/reportEmbed?reportId=56e166a1-79d9-412b-a783-7a8f897baf5a&autoAuth=true&ctid=a18d4da0-fa29-4ca0-80a3-dafe7e29cff3)💸

### Thank you for reading! 🤑 😄

