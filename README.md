# UK-Police-Recorded-Crime-Analysis
Analysis of England &amp; Wales police recorded crime data (2012/13 - 2023/24) using Microsoft Excel
A comprehensive data analysis project examining police recorded crime trends across England and Wales over 12 financial years, using Microsoft Excel for data cleaning, transformation, analysis, and visualisation.

📌 Project Overview

This project analyses 258,906 records of police recorded crime data published by the UK Home Office, covering 44 territorial police forces across 12 financial years from 2012/13 to 2023/24. The analysis explores national trends, seasonal patterns, geographic distribution, and offence category deep-dives.

🎯 Objectives

Merge and clean 12 separate year-sheets into a single unified dataset using Power Query
Identify long-term trends in total recorded crime across England and Wales
Analyse the impact of COVID-19 on crime volumes
Examine seasonal patterns in crime by financial quarter
Compare crime volumes and trends across all 44 territorial police forces
Perform statistical analysis (mean, median, standard deviation, correlation) by offence group

## 🗂️ Dataset
 
| Attribute | Detail |
|---|---|
| **Source** | UK Home Office – Police Recorded Crime |
| **Coverage** | England and Wales |
| **Period** | 2012/13 – 2023/24 (12 financial years) |
| **Records** | 258,906 rows |
| **Forces** | 44 territorial police forces |
| **Columns** | 9 (Financial Year, Quarter, Force, Offence Group, Subgroup, Description, Code, Count, Force Type) |

 
---
 
## 🛠️ Tools & Techniques
 
| Tool / Feature | Purpose |
|---|---|
| **Power Query** | Data import, cleaning, merging of 12 year-sheets, type conversion, trimming |
| **PivotTables** | Aggregation by year, force, offence group, and quarter |
| **Excel Charts** | Line, bar, stacked bar, and clustered bar visualisations |

## 📊 Key Findings
 
### 📈 National Trends
- Total recorded crime rose **65.8%** from 4.1 million (2012/13) to 6.7 million (2022/23)
- The upward trend was briefly interrupted in 2020/21 due to the COVID-19 pandemic, before recovering strongly in 2021/22 and continuing to rise through 2022/23.

### Total Recorded Crime Over Time
![](https://github.com/Bilqees-Oluwatoyin-Abdullahi/UK-Police-Recorded-Crime-Analysis/blob/main/Total%20recorded%20crime%20over%20time.png)
 

### 🦠 COVID-19 Impact
- Total crime fell **10.6%** in 2020/21 (from 6.08M to 5.43M offences) due to lockdown restrictions
- Crime rebounded strongly in 2021/22 (+16.7%) and continued rising through 2022/23

### COVID-19 Impact
![](https://github.com/Bilqees-Oluwatoyin-Abdullahi/UK-Police-Recorded-Crime-Analysis/blob/main/COVID%2019%20impact.png)


### 🗓️ Seasonal Patterns
- **Q1 (January–March) is the highest-crime quarter across virtually all years, with a total of 16,003,855 offences recorded across the full dataset.
- **Q4 (October–December) is consistently the lowest, with 14,231,724 total offences.

### Seasonal Pattern by Quarter
![](https://github.com/Bilqees-Oluwatoyin-Abdullahi/UK-Police-Recorded-Crime-Analysis/blob/main/Total%20Recorded%20Crime%20by%20Quarter.png)

### Average Quarterly Crime by Offence Group
- **Fraud offences** record the highest average quarterly volume by a significant margin, peaking in Q4 at ~21,000 offences per quarter — driven largely by national reporting bodies (Action Fraud, CIFAS) rather than territorial forces
- Seasonal variation between quarters is **minimal at the offence group level**, with all four quarters following near-identical trends across categories
- The Q1 national dominance observed in total crime figures is driven by **aggregate volume effects** rather than strong within-group seasonal patterns

![](https://github.com/Bilqees-Oluwatoyin-Abdullahi/UK-Police-Recorded-Crime-Analysis/blob/main/Average%20Quarterly%20Crime%20by%20Offence%20Group.png)


### 🗺️ Geographic Distribution
- The **Metropolitan Police** recorded the highest percentage across the period, with 33.35% of total recorded territorial crimes.
- The Met's national share has **declined over time** as regional forces record faster growth
- **West Midlands** and **West Yorkshire** form the next tier of high-volume forces each recording between 11.6% and 10.1% of total recorded territorial.

### Top 10 Police Forces
![](https://github.com/Bilqees-Oluwatoyin-Abdullahi/UK-Police-Recorded-Crime-Analysis/blob/main/Top%20Ten%20Police%20Forces%20by%20Percentage%20Recorded%20Crime.png)


### Offence Trends
- **Miscellaneous crimes against society** and **Violence against the person** both surpassed 2.1 million offences by 2022/23, overtaking Theft as the highest-volume groups
- **Theft offences** declined from being the highest group in 2012/13 (1.9M) and never fully recovered to pre-COVID levels after the 2020/21 lockdown dip
- **Fraud offences** grew consistently throughout the period (+126%), with COVID-19 having minimal impact — suggesting a shift to online fraud during lockdown
- **Public order offences** nearly doubled across the period, rising from ~150,000 to ~600,000 by 2022/23
- The sharp drop in 2023/24 across all groups reflects **incomplete data (Q1 only)** and does not represent a genuine downward trend

### Trends by Offence Group
![](https://github.com/Bilqees-Oluwatoyin-Abdullahi/UK-Police-Recorded-Crime-Analysis/blob/main/Trend%20by%20offence%20group.png) 


### 📐 Statistical Highlights
- Large gaps between mean and median values across all groups reflect significant **right-skew**, driven by high-volume forces
- **Fraud offences** have the highest standard deviation (19,176.6), reflecting concentration in national fraud reporting bodies
- **Violence and Sexual offences** show strong positive correlation, rising in tandem across the period


---


## ⚠️ Data Quality Notes
 
| Issue | Action Taken |
|---|---|
| 2016/17 columns incorrectly named | Corrected before merging |
| 2022/23 columns misarranged | Rearranged to match standard structure |
| Financial Quarter stored as text | Converted to Whole Number in Power Query |
| 426 rows with negative offence counts | Retained — represent legitimate Home Office recording reversals |
| 66,913 rows with zero offence counts | Retained — represent genuine absence of that crime type |
| No duplicate records found | Confirmed via Power Query deduplication |
| 2023/24 data incomplete (Q1 only) | Included in dataset but excluded from trend comparisons |
| CIFAS listed with inconsistent capitalisation | Standardised to "CIFAS" via Find & Replace |
 
---
 
## 📝 Workbook

The Merged data, analysis and dashboard ([Police_Recorded_Crime_Merged_Records.xlsx](https://github.com/Bilqees-Oluwatoyin-Abdullahi/UK-Police-Recorded-Crime-Analysis/blob/main/Police_Recorded_Crime_Merged_Records.xlsx))

## 📝 Report
 
The full written report ([Police_Crime_Analysis_Report.docx](https://github.com/Bilqees-Oluwatoyin-Abdullahi/UK-Police-Recorded-Crime-Analysis/blob/0c2f32cf3c78064e3d6eddfe2ba49f4704ca0435/Police_Crime_Analysis_Report.docx)) covers:
 
1. Executive Summary
2. Dataset Overview
3. National Trend Analysis
4. COVID-19 Impact Analysis
5. Seasonal Analysis
6. Geographic Analysis
7. Statistical Summary
8. Key Findings & Limitations
9. Conclusion & References
---

## 👩‍💻 Author
 
**Bilqis Oluwatoyin Abdullahi**
 
---
 
## 📜 Licence
 
The source data is published under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/). All analysis, visualisations, and written content in this repository are the original work of the author.
 
