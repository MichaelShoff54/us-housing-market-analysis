## Core Data Fields

| Field | Source | Description |
|---|---|---|
| RegionName | Zillow | Metropolitan area associated with each Zillow housing observation. |
| Date | Zillow | Monthly observation date for home value and housing inventory data. |
| Rent Date | Zillow | Monthly observation date for Zillow rent data. |
| Home Value | Zillow ZHVI | Typical home value for the metropolitan area based on the Zillow Home Value Index. |
| Rent | Zillow ZORI | Typical monthly market rent for the metropolitan area based on the Zillow Observed Rent Index. |
| Inventory | Zillow | Number of homes listed for sale within the metropolitan area. |
| Mortgage Rate | FRED | Average 30-year fixed mortgage rate. Weekly observations were transformed into monthly averages for historical analysis. |
| Median Household Income | U.S. Census Bureau ACS | 2024 ACS 5-Year Estimate of median household income for the metropolitan area. |
| Income Year | U.S. Census Bureau ACS | Reference year associated with the household income estimate. |
| Zillow Metro | Metro Crosswalk | Standardized Zillow metropolitan-area name used to connect housing and income data. |
| Census Metro | Metro Crosswalk | Census metropolitan-area name mapped to the corresponding Zillow metro. |

## Calculated Metrics

| Metric | Calculation / Methodology | Description |
|---|---|---|
| 2024 Home Value | December 2024 ZHVI | Typical home value used as the year-end 2024 affordability benchmark. |
| Monthly Rent | December 2024 ZORI | Typical monthly rent used for the 2024 affordability analysis. |
| Home Value Growth | (Dec. 2024 Home Value / Dec. 2023 Home Value) - 1 | Year-over-year percentage change in metro home values. |
| Rent Growth | (Dec. 2024 Rent / Dec. 2023 Rent) - 1 | Year-over-year percentage change in metro rents. |
| Price-to-Income Ratio | 2024 Home Value / Median Household Income | Measures the relationship between typical home values and annual household income. A higher ratio indicates lower relative affordability. |
| Estimated Mortgage P&I | 20% down, 30-year term, 6.724% annual interest rate | Estimated monthly principal and interest payment based on the December 2024 home value. Excludes taxes, insurance, HOA fees, maintenance, and other ownership costs. |
| Mortgage P&I % of Income | (Estimated Monthly Mortgage P&I × 12) / Median Household Income | Estimated percentage of annual household income required for mortgage principal and interest. |
| Rent % of Income | (Monthly Rent × 12) / Median Household Income | Estimated percentage of annual household income required for rent. |
| Investment Growth Score | (Home Value Growth + Rent Growth) / 2 | Custom metric combining home-value appreciation and rent growth with equal 50% weighting. Used to compare market momentum across metros. |
