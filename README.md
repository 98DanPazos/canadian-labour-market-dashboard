# Canadian Labour Market Dashboard

## Overview
A data analysis project examining trends in Canada's labour market using 
Statistics Canada Labour Force Survey (LFS) data (Table 14-10-0017-01). 
Covers national and provincial unemployment, participation trends, and 
labour market conditions by gender and age cohort from 2010 to present.

## Key Questions
- How has the national unemployment rate evolved over the past 15 years?
- How do unemployment rates differ by gender and age group?
- Which provinces currently have the tightest and loosest labour markets?

## Data Source
| Table | Source | Description |
|-------|--------|-------------|
| 14-10-0017-01 | Statistics Canada | Labour force characteristics by gender and detailed age group, monthly, unadjusted (x 1,000) |

Downloaded from: https://www150.statcan.gc.ca/t1/tbl1/en/dtbl/14-10-0017-01

## Key Findings (April 2026)
- National unemployment rate: **6.6%**
- Participation rate: **65.7%**
- Employment rate: **61.3%**
- Youth unemployment (15–24) remains elevated relative to prime-age workers (25–44)
- Men and women show converging unemployment rates compared to earlier decades

## Charts
| File | Description |
|------|-------------|
| 01_national_unemployment.png | National unemployment rate 2010–present |
| 02_unemployment_by_gender.png | Unemployment rate by gender 2010–present |
| 03_unemployment_by_age.png | Unemployment rate by age group, latest month |
| 04_provincial_unemployment.png | Unemployment rate by province, latest month |

## Methodology
Data filtered to 15+ age group, both sexes combined for national and 
provincial charts. Gender breakdown uses Men+ and Women+ categories as 
defined by Statistics Canada. All series are unadjusted for seasonality. 
Charts produced in Python using pandas and matplotlib.

## Limitations
- Unadjusted series — month-to-month movements reflect seasonal patterns 
  as well as underlying labour market conditions
- LFS is a household survey subject to sampling error, particularly at 
  the provincial level for smaller provinces
- Industry-level breakdown not included in this version

## Tools
Python 3.11 | pandas | matplotlib | seaborn | Jupyter

## Reproducing This Project
1. Download Table 14-10-0017-01 from Statistics Canada (link above)
2. Place the CSV in `data/raw/14100017.csv`
3. Run `notebooks/01_labour_dashboard.ipynb` top to bottom