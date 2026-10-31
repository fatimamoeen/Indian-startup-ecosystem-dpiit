# DPIIT Startup Ecosystem — Government Data Analysis & Interactive Dashboard
A student-led data analysis and visualization project exploring DPIIT-recognised startups, employment indicators, industry distribution and selected government startup-support schemes.

Tools: Python (Pandas) · Microsoft Excel · Power Query · PivotTables · PivotCharts · Slicers

Table of Contents
1. Project Overview
2. Project Objectives
3. Data Sources and Coverage
4. Types of Data Handled
5. Data Preparation and Workflow
6. Excel Dashboard
7. Key Insights
8. How the Analysis Can Support Policy Discussions
9. Project Structure
10. Limitations
11. Conclusion
12. Sources
Project Overview
India’s startup ecosystem is represented across several government datasets and parliamentary disclosures. These sources contain information on DPIIT startup recognition, state and industry distribution, employment indicators, and financial support provided through different schemes.

This project brings selected datasets into a structured analysis and an interactive Excel dashboard. Python (Pandas) is used for data inspection and preparation, while Excel and Power Query are used to organize, compare and visualize the information.

The objective is to make government data easier to explore and interpret. The dashboard is intended to support descriptive analysis and policy discussions by helping users examine where recognised startups are located, which industries are represented, and how different forms of financial support are distributed.

This is an independent student project based on publicly available government information. It is not an official DPIIT publication or an evaluation of scheme impact.
Project Objectives
- Organize public data on DPIIT-recognised startups across states/UTs, years and industries.
- Examine reported employment indicators alongside startup recognition data, while keeping their reporting periods clear.
- Explore state-wise distribution of support under FFS, SISFS and CGSS.
- Build an interactive dashboard that makes the data easier to filter, compare and communicate.
- Identify descriptive patterns that may help frame further questions for policy research and programme review.
Data Sources and Coverage
Source / file used	Information handled	Coverage / reporting basis	Main use in the project
DPIIT_Statewise_Startup_Recognition_2016_2022.csv	DPIIT-recognised startup counts by State/UT and year	2016–2022; 36 State/UT rows; total of 84,012 in the supplied state-wise file	State rankings, recognition trends and geographic concentration
EMPLOYED NEW.csv	State/UT-wise number of employees	Self-reported employment total of 863,608 as of 30 November 2022	Employment indicator and state-wise comparison
RAJYA SABHA.pdf — Unstarred Question No. 542	Startup recognition, industry distribution, FFS/AIF investment, SISFS approvals and CGSS loan guarantees	Answered 7 February 2025; annexure data generally through 31 December 2024	More recent recognition and scheme-level context
Supplementary allocation/utilisation table in the workbook	Amount allocated to selected incubators and amount utilised	Values currently present in the workbook; exact source URL and extraction date still need to be attached	Supporting allocation-versus-utilisation visualization


The OGD Platform India catalog titled Startup Recognized by DPIIT describes the broader government dataset as containing startup counts by year, sector and state. The workbook also uses an earlier state-wise extract covering 2016–2022 and a later parliamentary response for 2020–2024 and scheme details. These are treated as separate reporting snapshots rather than forced into one continuous series.
Types of Data Handled
Data type	Examples of fields	Why it matters
Time-series counts	Recognition counts by year	Helps observe how annual recognition volumes change over time
Geographic data	State/UT names and startup counts	Enables state-wise ranking and comparison
Industry data	Industry categories and yearly startup counts	Shows the spread of recognised startups across sectors
Employment indicators	Self-reported number of employees / direct jobs	Adds an employment dimension to the ecosystem overview
Scheme-level support data	Startups selected, loans guaranteed, borrowers	Shows the reach of different government support mechanisms
Financial data	Investment, approved amount, allocated amount, utilised amount, loan guarantees (₹ crore)	Supports comparisons of financial support, with each financial measure kept distinct


Data Preparation and Workflow
The project follows a practical data-to-dashboard workflow:
1. Source collection: Collected government datasets and tables from official DPIIT / OGD resources, PIB material and parliamentary replies.
2. Initial inspection in Python: Used Pandas to inspect column names, data types, missing values and duplicate records.
3. Cleaning and structuring: Prepared numeric fields for analysis, reviewed missing entries, and standardized State/UT labels where tables needed to be compared.
4. Power Query preparation: Used Excel Power Query to import and transform separate data tables into a more consistent structure for dashboard reporting.
5. Analysis: Summarized counts and amounts by year, State/UT, industry and scheme. Tables with different reporting periods or definitions were kept separate where a direct comparison would be misleading.
6. Dashboard development: Used Excel tables, PivotTables, PivotCharts, formulas and slicers to present the information in an interactive format.
7. Review: Checked totals against the source tables and noted differences that need reconciliation before external publication.
Tools and features
Tool	How it was used
Python — Pandas	Data loading, inspection, missing-value and duplicate checks, type review, cleaning and preparation
Microsoft Excel	Data organization, calculations, summary tables and dashboard presentation
Power Query	Importing and transforming multiple source tables
PivotTables / PivotCharts	Summarising and visualising state-wise, industry-wise and scheme-wise information
Slicers	Filtering dashboard views interactively
Excel formulas	KPI calculations and supporting summary values


Excel Dashboard
The dashboard brings the prepared data into one visual interface. It includes:
- KPI cards for headline indicators.
- State-wise and industry-wise startup recognition views.
- Employment and scheme-support comparisons.
- Funding / investment and loan-guarantee summaries.
- Tables for year-wise recognition and reported jobs.
- Slicers to filter selected dashboard views.
The dashboard is designed to make it easier to explore the data without reading every underlying table. It supports comparison and interpretation; it does not itself establish why a state or sector has a particular outcome.
Key Insights
A few quick observations from the available datasets and the Rajya Sabha reply:
Area	Key observation
State-wise recognition	The top 10 states account for 68,803 of 84,012 recognitions (81.9%) in the supplied 2016–2022 state-wise dataset.
Year-wise recognition	Annual recognitions rose from 14,852 in 2020 to 34,842 in 2023, followed by 34,294 in 2024.
Industry-wise recognition	The five largest industry categories account for 13,139 recognitions (38.3%) of the 2024 total.
Financial support	The source reports ₹18,632.98 crore invested by AIFs under FFS, ₹467.75 crore approved under SISFS, and ₹601.86 crore in CGSS loan guarantees.


These comparisons help explore where DPIIT-recognised startups are located, which industries have a larger presence, and how different forms of startup support are distributed. They are descriptive observations, not proof of scheme impact or causes behind the patterns.
How the Analysis Can Support Policy Discussions
The dashboard can serve as an accessible starting point for questions such as:
- Regional ecosystem development: Which states have higher startup recognition, and where might further investigation into ecosystem access be useful?
- Sector-specific support: Which industries have a larger presence, and do their needs differ in areas such as incubation, infrastructure, skills or market access?
- Geographic access to finance: Are AIF investments, seed-fund approvals and credit guarantees concentrated in the same states, or do their distributions differ
Limitations
- Several datasets have different reporting dates and coverage periods.
- Some indicators are self-reported by recognised startups.
- Recognition counts describe DPIIT recognition, not all businesses or all startups operating in India.
- Scheme measures are not interchangeable: AIF investment, incubator-approved amounts and credit guarantees represent different forms of support.
- State-level concentration is descriptive; it does not explain the reasons behind the distribution.
- The analysis does not establish whether a scheme caused an increase in startup formation, employment or investment.
- Small differences exist between some workbook subtotals and official annexure totals, as described above.
- DPIIT-Startup-Ecosystem/
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
Conclusion
This project converts multiple public datasets and parliamentary disclosures into a structured, interactive view of India’s startup ecosystem. By examining startup recognition, industry distribution, employment indicators and different forms of financial support, it makes patterns easier to explore and provides a starting point for evidence-based policy discussions.
Sources
1. Open Government Data (OGD) Platform India — Startup Recognized by DPIIT: data.gov.in/catalog/startup-recognized-dpiit
2. PIB — DPIIT-recognised startups and self-reported jobs as of 30 November 2022: Press Release PRID 1884256
3. Lok Sabha Unstarred Question No. 35 — Startup India, 7 December 2022: Official Sansad annexure PDF
4. Rajya Sabha Unstarred Question No. 542 — Startup India Scheme, 7 February 2025: Official Sansad PDF
- Programme monitoring: How do the reported reach and financial values of FFS, SISFS and CGSS compare when their different mechanisms and time periods are kept clear?
- Inclusion indicators: What does the self-reported woman director/partner indicator show, and what additional data would be needed to understand participation more fully?
These are potential uses of the analysis. The project is descriptive and does not establish causal relationships or measure the impact of individual schemes.
