# U.S. Housing Market Investment & Affordability Analysis

An interactive Tableau data analytics project examining housing market trends, affordability, and investment growth across U.S. metropolitan areas.

## Project Overview

This project combines housing, rental, inventory, mortgage rate, and household income data to evaluate conditions across U.S. housing markets.

The analysis was designed to answer three primary questions:

1. How have home values, rents, housing inventory, and mortgage rates changed over time?
2. How affordable are U.S. metropolitan housing markets relative to household income?
3. Which metropolitan areas demonstrate the strongest combination of home value appreciation and rental growth?

The project includes three interactive analytical dashboards:

- **U.S. Housing Market Overview** — Historical home value, rent, inventory, and mortgage-rate trends.
- **Housing Affordability Analysis** — Home values and housing costs compared with household income.
- **Market Investment Explorer** — Metro-level comparison of home value growth, rent growth, affordability, and market momentum.

## Tools & Skills

**Tableau** — Dashboard development, calculated fields, parameters, filters, relationships, KPI reporting, and interactive data visualization.

**Excel / Power Query** — Data cleaning, transformation, unpivoting, aggregation, and preparation of analysis-ready datasets.

**Data Modeling** — Integrated Zillow, Census, and FRED data using a custom metropolitan-area crosswalk.

**Financial Analysis** — Housing affordability ratios, estimated mortgage payments, income burden metrics, and market growth analysis.

## Dashboard Preview

### U.S. Housing Market Overview

Tracks metro-level home values, rents, housing inventory, and national mortgage rates over time.

![U.S. Housing Market Overview](screenshots/Housing_Market_Overview.png)

### Housing Affordability Analysis

Compares home values, household income, rent, and estimated mortgage costs to evaluate housing affordability across U.S. metropolitan areas.

![Housing Affordability Analysis](screenshots/US_Housing_Affordability_Analysis.png)

### Market Investment Explorer

Compares home value growth, rent growth, affordability, and a custom Investment Growth Score to identify markets demonstrating strong housing and rental momentum.

![Market Investment Explorer](screenshots/Market_Investment_Explorer.png)

### Methodology & Data Sources

Documents the datasets, calculations, assumptions, data preparation process, and analytical limitations used throughout the project.

![Methodology & Data Sources](screenshots/Methodology_and_Sources.png)

## Data Sources

This analysis integrates five datasets from three primary sources:

- **Zillow Research — Zillow Home Value Index (ZHVI):** Metro-level typical home values.
- **Zillow Research — Zillow Observed Rent Index (ZORI):** Metro-level typical monthly rents.
- **Zillow Research — For-Sale Inventory:** Metro-level housing inventory.
- **Federal Reserve Economic Data (FRED) — MORTGAGE30US:** 30-year fixed mortgage rates.
- **U.S. Census Bureau — ACS 5-Year B19013:** 2024 median household income by metropolitan area.

## Methodology

Housing datasets were cleaned and transformed in Excel Power Query, including reshaping monthly data into analysis-ready tables. Weekly mortgage-rate observations were aggregated into monthly averages.

A custom metro crosswalk was created to integrate Census household income data with Zillow metropolitan-area data despite differences in geographic naming conventions.

For the 2024 affordability analysis:

- Home values and rents use December 2024 observations.
- Household income uses the 2024 ACS 5-Year Estimate.
- Estimated mortgage payments assume a 20% down payment, 30-year fixed-rate term, and 6.724% average 2024 mortgage rate.
- Mortgage estimates represent principal and interest only.
- Investment Growth Score equally weights 2024 home value growth and rent growth.

For detailed field definitions and calculation methodology, see [`documentation/DATA_DICTIONARY.md`](documentation/DATA_DICTIONARY.md).



