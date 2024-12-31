# The World Bank's International Debt Data Analysis

This repository contains an exploratory data analysis project focused on international debt data provided by the [World Bank](https://www.worldbank.org). The aim of this project is to investigate the amount of debt owed by various developing countries across different debt categories. The data is stored in a PostgreSQL database (table named `international_debt`), and all analyses are conducted using SQL queries.

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Dataset Description](#dataset-description)  
3. [Analysis Steps](#analysis-steps)  
4. [Key Findings](#key-findings)  
5. [Getting Started](#getting-started)  
6. [Contact](#contact)

---

## Project Overview

Economies worldwide rely on various forms of debt to sustain growth and manage shortfalls. Developing countries, in particular, often rely on debt to fund infrastructure, social programs, and other initiatives that support economic development. By analyzing the World Bank’s international debt data, we aim to:

- Understand how many countries are represented in the dataset.
- Identify the different debt indicators and their purposes.
- Calculate the total global debt from all countries in the dataset.
- Determine which countries owe the most and in which categories.
- Explore indicators with the highest average debt.
- Examine which debt indicators are most common across all countries.

---

## Dataset Description

- **Source**: [World Bank’s International Debt Data](https://www.worldbank.org/)
- **Table**: `international_debt`
- **Fields**:
  - `country_name`: Name of the country.
  - `indicator_name`: Brief description of the debt category.
  - `indicator_code`: Code representing the category of debt.
  - `debt`: Amount of debt (in USD).

*Note*: The table has multiple rows for each country since each country can have debt in more than one category.

---

## Analysis Steps

Below is a brief outline of the SQL queries and analyses performed:

1. **Initial Exploration**  
   - Selected the first 10 rows to get a preview of the dataset.

2. **Distinct Countries**  
   - Counted the number of unique countries in the dataset using `COUNT(DISTINCT country_name)`.

3. **Distinct Debt Indicators**  
   - Extracted the different debt indicators to understand how debt categories are grouped.

4. **Total Debt Calculation**  
   - Summed the debt (in USD) across all countries to see the overall global debt figure.

5. **Highest Debt by Country**  
   - Determined which country has the maximum total debt across all indicators combined.

6. **Average Debt by Indicator**  
   - Computed the average debt (in USD) for each debt indicator to gauge which categories tend to have higher or lower debt amounts.

7. **Highest Amount of Principal Repayments**  
   - Focused specifically on the indicator `DT.AMT.DLXF.CD` (long-term debt) to find out which country owes the highest amount in this category.

8. **Most Common Debt Indicator**  
   - Discovered which indicator appears most frequently among all countries.

9. **Maximum Debt Across Indicators**  
   - Identified, for each indicator, the country that owes the highest amount.

---

## Key Findings

1. **Total Number of Countries**: There are 124 distinct countries represented in the dataset.  
2. **Total Global Debt**: Summed to over 3 million million USD (i.e., trillions).  
3. **Country with the Highest Overall Debt**: China emerges as the country with the largest total debt.  
4. **Indicators with the Highest Average Debt**:
   - `DT.AMT.DLXF.CD` (long-term debt) tops the average debt chart.
   - Followed by `DT.DIS.DLXF.CD`, indicating that long-term debt issuance is also significant.
5. **Country with the Highest Long-Term Debt**: China also leads in the `DT.AMT.DLXF.CD` category.
6. **Most Common Debt Indicator**: The SQL queries revealed which indicator (by code) occurs most frequently, helping to understand commonalities in global debt structures.

---

## Getting Started

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/your-username/your-repo-name.git

  ---

## Contact

If you have any questions or suggestions, feel free to reach out via GitHub Issues or contact me at [LinkedIn](https://www.linkedin.com/in/binita-roy/)|[GitHub](https://github.com/binita-roy).
