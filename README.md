# 🇮🇳 DPIIT Startup Ecosystem — Government Data Analysis & Interactive Dashboard

> **A student-led data analysis and visualization project** exploring DPIIT-recognised startups, employment indicators, industry distribution and selected government startup-support schemes.
>
> **Tools:** Python (Pandas) · Microsoft Excel · Power Query · PivotTables · PivotCharts · Slicers

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Project Objectives](#project-objectives)
3. [Data Sources and Coverage](#data-sources-and-coverage)
4. [Types of Data Handled](#types-of-data-handled)
5. [Data Preparation and Workflow](#data-preparation-and-workflow)
6. [Excel Dashboard](#excel-dashboard)
7. [Key Insights](#key-insights)
   - [Startup Recognition by State](#1-startup-recognition-by-state-20162022)
   - [Annual Recognition Trend](#2-annual-recognition-trend-20202024)
   - [Industry Distribution](#3-industry-distribution-in-2024)
   - [Fund of Funds for Startups](#4-fund-of-funds-for-startups-ffs)
   - [Startup India Seed Fund Scheme](#5-startup-india-seed-fund-scheme-sisfs)
   - [Credit Guarantee Scheme for Startups](#6-credit-guarantee-scheme-for-startups-cgss)
   - [Employment and Women’s Participation Indicators](#7-employment-and-womens-participation)
8. [How the Analysis Can Support Policy Discussions](#how-the-analysis-can-support-policy-discussions)
9. [Project Structure](#project-structure)
10. [Limitations](#limitations)
11. [Conclusion](#conclusion)
12. [Sources](#sources)

---

## Project Overview

India’s startup ecosystem is represented across several government datasets and parliamentary disclosures. These sources contain information on DPIIT startup recognition, state and industry distribution, employment indicators, and financial support provided through different schemes.

This project brings selected datasets into a structured analysis and an interactive Excel dashboard. Python (Pandas) is used for data inspection and preparation, while Excel and Power Query are used to organize, compare and visualize the information.

The objective is to make government data easier to explore and interpret. The dashboard is intended to support descriptive analysis and policy discussions by helping users examine where recognised startups are located, which industries are represented, and how different forms of financial support are distributed.

**This is an independent student project based on publicly available government information. It is not an official DPIIT publication or an evaluation of scheme impact.**

## Project Objectives

- Organize public data on DPIIT-recognised startups across states/UTs, years and industries.
- Examine reported employment indicators alongside startup recognition data, while keeping their reporting periods clear.
- Explore state-wise distribution of support under FFS, SISFS and CGSS.
- Build an interactive dashboard that makes the data easier to filter, compare and communicate.
- Identify descriptive patterns that may help frame further questions for policy research and programme review.

## Data Sources and Coverage

| Source / file used | Information handled | Coverage / reporting basis | Main use in the project |
|---|---|---|---|
| `DPIIT_Statewise_Startup_Recognition_2016_2022.csv` | DPIIT-recognised startup counts by State/UT and year | 2016–2022; 36 State/UT rows; total of 84,012 in the supplied state-wise file | State rankings, recognition trends and geographic concentration |
| `EMPLOYED NEW.csv` | State/UT-wise number of employees | Self-reported employment total of 863,608 as of 30 November 2022 | Employment indicator and state-wise comparison |
| `RAJYA SABHA.pdf` — Unstarred Question No. 542 | Startup recognition, industry distribution, FFS/AIF investment, SISFS approvals and CGSS loan guarantees | Answered 7 February 2025; annexure data generally through 31 December 2024 | More recent recognition and scheme-level context |
| Supplementary allocation/utilisation table in the workbook | Amount allocated to selected incubators and amount utilised | Values currently present in the workbook; exact source URL and extraction date still need to be attached | Supporting allocation-versus-utilisation visualization |

The OGD Platform India catalog titled **Startup Recognized by DPIIT** describes the broader government dataset as containing startup counts by year, sector and state. The workbook also uses an earlier state-wise extract covering 2016–2022 and a later parliamentary response for 2020–2024 and scheme details. These are treated as separate reporting snapshots rather than forced into one continuous series.

## Types of Data Handled

| Data type | Examples of fields | Why it matters |
|---|---|---|
| Time-series counts | Recognition counts by year | Helps observe how annual recognition volumes change over time |
| Geographic data | State/UT names and startup counts | Enables state-wise ranking and comparison |
| Industry data | Industry categories and yearly startup counts | Shows the spread of recognised startups across sectors |
| Employment indicators | Self-reported number of employees / direct jobs | Adds an employment dimension to the ecosystem overview |
| Scheme-level support data | Startups selected, loans guaranteed, borrowers | Shows the reach of different government support mechanisms |
| Financial data | Investment, approved amount, allocated amount, utilised amount, loan guarantees (₹ crore) | Supports comparisons of financial support, with each financial measure kept distinct |

## Data Preparation and Workflow

The project follows a practical data-to-dashboard workflow:

1. **Source collection:** Collected government datasets and tables from official DPIIT / OGD resources, PIB material and parliamentary replies.
2. **Initial inspection in Python:** Used Pandas to inspect column names, data types, missing values and duplicate records.
3. **Cleaning and structuring:** Prepared numeric fields for analysis, reviewed missing entries, and standardized State/UT labels where tables needed to be compared.
4. **Power Query preparation:** Used Excel Power Query to import and transform separate data tables into a more consistent structure for dashboard reporting.
5. **Analysis:** Summarized counts and amounts by year, State/UT, industry and scheme. Tables with different reporting periods or definitions were kept separate where a direct comparison would be misleading.
6. **Dashboard development:** Used Excel tables, PivotTables, PivotCharts, formulas and slicers to present the information in an interactive format.
7. **Review:** Checked totals against the source tables and noted differences that need reconciliation before external publication.

### Tools and features

| Tool | How it was used |
|---|---|
| Python — Pandas | Data loading, inspection, missing-value and duplicate checks, type review, cleaning and preparation |
| Microsoft Excel | Data organization, calculations, summary tables and dashboard presentation |
| Power Query | Importing and transforming multiple source tables |
| PivotTables / PivotCharts | Summarising and visualising state-wise, industry-wise and scheme-wise information |
| Slicers | Filtering dashboard views interactively |
| Excel formulas | KPI calculations and supporting summary values |

## Excel Dashboard

The dashboard brings the prepared data into one visual interface. It includes:

- KPI cards for headline indicators.
- State-wise and industry-wise startup recognition views.
- Employment and scheme-support comparisons.
- Funding / investment and loan-guarantee summaries.
- Tables for year-wise recognition and reported jobs.
- Slicers to filter selected dashboard views.

The dashboard is designed to make it easier to explore the data without reading every underlying table. It supports comparison and interpretation; it does not itself establish why a state or sector has a particular outcome.

## Key Insights

The findings below are descriptive calculations from the supplied workbook tables and the official parliamentary source. The reporting periods are stated alongside the figures because the source datasets do not all use the same snapshot date.

### 1. Startup Recognition by State (2016–2022)

The supplied state-wise recognition file contains **84,012 recognised startups** across 36 State/UT rows for 2016–2022. The ten highest-count states account for **68,803 startups, or approximately 81.9%** of the dataset total.

| Rank | State / UT | Recognised startups | Share of 84,012 |
|---:|---|---:|---:|
| 1 | Maharashtra | 15,571 | 18.5% |
| 2 | Karnataka | 9,904 | 11.8% |
| 3 | Delhi | 9,588 | 11.4% |
| 4 | Uttar Pradesh | 7,719 | 9.2% |
| 5 | Gujarat | 5,877 | 7.0% |
| 6 | Tamil Nadu | 4,704 | 5.6% |
| 7 | Haryana | 4,511 | 5.4% |
| 8 | Telangana | 4,426 | 5.3% |
| 9 | Kerala | 3,764 | 4.5% |
| 10 | West Bengal | 2,739 | 3.3% |

**What this suggests:** In this 2016–2022 state-wise dataset, startup recognition is concentrated in a relatively small group of states. This can help identify where further research into ecosystem infrastructure, access to networks, capital and support services may be useful. The figures alone do not explain the reasons for the concentration.

### 2. Annual Recognition Trend (2020–2024)

The Rajya Sabha reply to Unstarred Question No. 542 reports the following annual number of DPIIT-recognised entities by year, as on 31 December 2024.

| Year | Recognitions | Year-on-year change |
|---:|---:|---:|
| 2020 | 14,852 | — |
| 2021 | 20,282 | +36.6% |
| 2022 | 26,596 | +31.1% |
| 2023 | 34,842 | +31.0% |
| 2024 | 34,294 | −1.6% |

**What this suggests:** Annual recognitions increased strongly between 2020 and 2023, while the 2024 count was slightly below 2023. These are annual recognition counts, not cumulative totals. The change is a descriptive trend and does not, by itself, indicate the cause of the movement.

### 3. Industry Distribution in 2024

The 2024 industry-wise table in Annexure II lists 55 industry categories. The five largest categories in the source table are:

| Industry | Recognised startups in 2024 |
|---|---:|
| IT Services | 3,538 |
| Healthcare & Lifesciences | 3,031 |
| Construction | 2,477 |
| Agriculture | 2,153 |
| Food & Beverages | 1,940 |
| **Combined** | **13,139** |

The five categories together represent approximately **38.3%** of the official 2024 total of 34,294.

**What this suggests:** IT Services is the largest single category in the 2024 table, but the recognised startup base is spread across multiple industries. The distribution can help frame sector-specific questions about support needs, market access, skills and infrastructure.

### 4. Fund of Funds for Startups (FFS)

Under FFS, SIDBI provides capital to SEBI-registered Alternative Investment Funds (AIFs), which in turn invest in startups. The parliamentary annexure reports the following state-wise AIF investment data for 2020–2024:

| Indicator | Reported value |
|---|---:|
| Startups selected by AIFs | 924 |
| Total amount invested by AIFs | ₹18,632.98 crore |

The three largest state-level investment amounts are Karnataka (₹5,692.50 crore), Maharashtra (₹4,380.77 crore) and Delhi (₹2,733.01 crore). Together, they account for approximately **68.7%** of the reported AIF investment total.

**What this suggests:** AIF investment is concentrated in a few major startup locations. This creates a useful policy-research question about geographic access to venture capital and the conditions that help startups attract investment. The amount shown is investment by AIFs in startups, not the Government’s direct disbursement to each startup.

### 5. Startup India Seed Fund Scheme (SISFS)

SISFS provides financial assistance to seed-stage startups through selected incubators. The scheme data covers 2021–2024.

| Indicator | Official parliamentary total |
|---|---:|
| Startups selected by incubators | 2,622 |
| Amount approved to selected startups | ₹467.75 crore |

Maharashtra, Karnataka and Tamil Nadu account for **1,069 selected startups**, approximately **40.8%** of the total. Their combined approved amount is ₹202.84 crore, approximately **43.4%** of the official approved amount.

**What this suggests:** Incubator-based seed support is distributed across many states, while the largest three states account for a substantial share of selections and approvals. State-level comparisons can help identify where incubator networks or seed-stage access may merit closer examination. Approved amounts should not be described as amounts disbursed unless disbursement data is separately available.

### 6. Credit Guarantee Scheme for Startups (CGSS)

CGSS enables collateral-free loans to startups through eligible financial institutions. The parliamentary annexure covers 2023–2024.

| Indicator | Official parliamentary total |
|---|---:|
| Loans guaranteed | 257 |
| Amount guaranteed | ₹601.86 crore |
| Unique borrowers supported | 206 |

Maharashtra recorded the highest state-wise amount guaranteed at ₹124.74 crore across 57 loans. The five largest state amounts (Maharashtra, Haryana, Tamil Nadu, Karnataka and Delhi) total ₹397.76 crore, approximately **66.1%** of the total guaranteed amount.

**What this suggests:** The state-wise guarantee data can help examine where credit-guarantee support is being accessed. A guarantee is not the same as a loan disbursement; the dashboard therefore treats the reported amounts as guarantees.

### 7. Employment and Women’s Participation

| Indicator | Reported value | Reporting basis |
|---|---:|---|
| Direct jobs created | 863,608 | Self-reported by DPIIT-recognised startups as of 30 November 2022 |
| Direct jobs created | Over 17.2 lakh | Reported in the Rajya Sabha reply as of 31 December 2024 |
| DPIIT-recognised entities | 1,57,706 | As of 31 December 2024 |
| Entities reporting at least one woman director/partner | 75,935 | Self-reported; as of 31 December 2024 |

The last two figures imply that approximately **48.1%** of recognised entities had self-reported at least one woman director/partner. This is not the percentage of women founders, women employees, or necessarily women-led startups; it is the specific indicator reported in the parliamentary reply.

The 2022 employment total and the 2024 jobs figure come from different reporting dates. They should not be presented as if they were the same snapshot.

## How the Analysis Can Support Policy Discussions

The dashboard can serve as an accessible starting point for questions such as:

- **Regional ecosystem development:** Which states have higher startup recognition, and where might further investigation into ecosystem access be useful?
- **Sector-specific support:** Which industries have a larger presence, and do their needs differ in areas such as incubation, infrastructure, skills or market access?
- **Geographic access to finance:** Are AIF investments, seed-fund approvals and credit guarantees concentrated in the same states, or do their distributions differ?
- **Programme monitoring:** How do the reported reach and financial values of FFS, SISFS and CGSS compare when their different mechanisms and time periods are kept clear?
- **Inclusion indicators:** What does the self-reported woman director/partner indicator show, and what additional data would be needed to understand participation more fully?

These are potential uses of the analysis. The project is descriptive and does not establish causal relationships or measure the impact of individual schemes.



## Project Structure

A suggested GitHub repository layout:

DPIIT-Startup-Ecosystem/
│
├── README.md
│
├── Source/
│   └── Rajya_Sabha_Startup_India_Scheme.pdf
│
├── Excel/
│   └── DPIIT_Startup_Ecosystem_Dashboard.xlsx
│       ├── Raw Data
│       ├── Calculations
│       ├── Analysis Tables
│       └── Interactive Dashboard
│
└── Poster/
    └── DPIIT_Startup_Ecosystem_Poster.html
```

Only include source files that you are permitted to redistribute. Otherwise, keep the official source links in this README and provide instructions for accessing them.

## Limitations

- Several datasets have different reporting dates and coverage periods.
- Some indicators are self-reported by recognised startups.
- Recognition counts describe DPIIT recognition, not all businesses or all startups operating in India.
- Scheme measures are not interchangeable: AIF investment, incubator-approved amounts and credit guarantees represent different forms of support.
- State-level concentration is descriptive; it does not explain the reasons behind the distribution.
- The analysis does not establish whether a scheme caused an increase in startup formation, employment or investment.
- Small differences exist between some workbook subtotals and official annexure totals, as described above.

## Conclusion

This project converts multiple public datasets and parliamentary disclosures into a structured, interactive view of India’s startup ecosystem. By examining startup recognition, industry distribution, employment indicators and different forms of financial support, it makes patterns easier to explore and provides a starting point for evidence-based policy discussions.

## Sources

1. **Open Government Data (OGD) Platform India — Startup Recognized by DPIIT:** [data.gov.in/catalog/startup-recognized-dpiit](https://data.gov.in/catalog/startup-recognized-dpiit)
2. **PIB — DPIIT-recognised startups and self-reported jobs as of 30 November 2022:** [Press Release PRID 1884256](https://www.pib.gov.in/PressReleasePage.aspx?PRID=1884256&lang=2&reg=48)
3. **Lok Sabha Unstarred Question No. 35 — Startup India, 7 December 2022:** [Official Sansad annexure PDF](https://sansad.in/getFile/loksabhaquestions/annex/1710/AU35.pdf?source=pqals)
4. **Rajya Sabha Unstarred Question No. 542 — Startup India Scheme, 7 February 2025:** [Official Sansad PDF](https://www.sansad.in/getFile/annex/267/AU542_5jBqtz.pdf?source=pqars)

---

*Prepared as a student data-analysis project. All calculated percentages are derived from the cited counts and amounts; rounding may cause small differences. Source definitions and reporting periods should be retained when reusing any figure.*

