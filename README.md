# healthcare-operations-financial-intelligence
#  Healthcare Operations & Financial Intelligence Dashboard

### Power BI Portfolio Project | AnalystLab Africa — Track A

## Project Overview

Hospitals generate large amounts of information about patient visits, medical procedures and healthcare costs. Analysing this information can help hospital managers understand service demand, manage resources and make better financial decisions.

This project uses **Microsoft Power BI** to analyse healthcare records and answer eight business questions covering hospital operations, claim costs, insurance coverage and procedure utilisation.

The results are presented in a three-page interactive dashboard.

## Business Objectives

The project aims to answer the following questions:

1. How have encounter volumes changed over time?
2. Which encounter classes account for the largest proportion of encounters?
3. What proportion of encounters lasted more than 24 hours, where valid timestamps are available?
4. Which encounter classes contribute the highest total claim costs?
5. How much of the total claim cost is covered by insurance payers?
6. Which procedures are performed most frequently?
7. Which procedures have the highest average base costs?
8. How do average claim costs differ across insurance payers?

The overall goal is to identify useful patterns and provide recommendations for healthcare operations and financial management.

---

## Tools Used

- **Power BI Desktop:** Dashboard development and interactive reporting.
- **Power Query:** Data cleaning and preparation.
- **DAX:** Measures and KPI calculations.
- **Data Modelling:** Relationships between healthcare datasets.
- **Data Visualisation:** Presenting findings through charts, cards and tables.

## Data Sources

The project uses five healthcare datasets:

| Dataset | Description |
|---|---|
| Encounters | Hospital visits, encounter classes, dates and claim costs |
| Patients | Patient information |
| Procedures | Medical procedures and base costs |
| Payers | Insurance payer information |
| Organizations | Healthcare organisation information |

### Data Preparation and Modelling

The datasets were prepared in Power Query by assigning appropriate data types, reviewing missing information and organising the tables for analysis.

Relationships were created between encounters, patients, procedures, payers and organisations.

A Date table was also created to support yearly and monthly reporting.

DAX measures were developed to calculate encounter volumes, unique patients, claim costs, payer coverage, procedure frequency and average costs.

---

# Dashboard Overview

The report contains three pages:

### Page 1 — Healthcare Operations Overview

Focuses on hospital encounter volumes, encounter classes, monthly patterns and encounter duration.

<img width="662" height="372" alt="Overview" src="https://github.com/user-attachments/assets/4aa62d67-4f76-42c3-8dc0-0db3a0d09448" />


### Page 2 — Healthcare Cost & Coverage Analysis

Focuses on total claim costs, insurance coverage, financial trends and payer performance.

<img width="664" height="379" alt="Financials" src="https://github.com/user-attachments/assets/0d094013-38ea-405b-90e7-e0f0192a77ab" />


### Page 3 — Procedure Utilisation & Cost Analysis

Focuses on procedure frequency, average base costs and resource planning.

<img width="666" height="381" alt="Procedures" src="https://github.com/user-attachments/assets/dd49b068-ccdf-4714-9d13-5e7c3152b62c" />


---

# Business Questions and Key Findings

## 1. How Have Encounter Volumes Changed Over Time?

**Total Encounters: 27,891**

The yearly encounter trend shows that hospital activity increased between 2011 and 2014.

Encounter volumes reached a high point in **2014**, remained relatively stable over the following years and increased again in **2021**.

The chart shows a sharp decrease in 2022, which should be interpreted in the context of the reporting period.

**Key Finding:** Hospital encounter volumes changed over time, with noticeable increases in 2014 and 2021.

**Business Importance:** Understanding encounter trends helps hospital management plan staffing and resources for periods of higher activity.

<img width="882" height="495" alt="Trends over time" src="https://github.com/user-attachments/assets/8d7d4481-d86c-42ca-945f-9b6b68179705" />


## 2. Which Encounter Classes Account for the Largest Proportion?

The dashboard shows the following encounter distribution:

| Encounter Class | Percentage |
|---|---:|
| Ambulatory | 44.95% |
| Outpatient | 22.59% |
| Urgent Care | 13.14% |
| Emergency | 8.33% |
| Wellness | 6.92% |
| Inpatient | 4.07% |

Ambulatory encounters account for the largest proportion of hospital visits, followed by outpatient encounters.

Together, these two categories represent approximately **67.5% of all encounters**.

**Key Finding:** Most recorded hospital encounters are ambulatory and outpatient visits.

<img width="884" height="499" alt="image" src="https://github.com/user-attachments/assets/57977c6c-2e46-425f-890c-3544d6acb2b4" />


## 3. What Proportion of Encounters Lasted More Than 24 Hours?

The encounter-duration analysis shows that **75 encounters**, representing approximately **0.27%**, lasted more than 24 hours.

The analysis considers encounters with valid start and end timestamps.

**Key Finding:** Only a small proportion of recorded encounters lasted longer than 24 hours.

**Business Importance:** Monitoring longer encounters can help management identify cases that may require additional attention or resources.

## 4. Which Encounter Classes Contribute the Highest Total Claim Costs?

**Total Claim Cost: $101.51 million**

The dashboard shows the following approximate claim costs:

| Encounter Class | Total Claim Cost |
|---|---:|
| Ambulatory | $36M |
| Urgent Care | $23M |
| Outpatient | $14M |
| Emergency | $11M |
| Inpatient | $9M |
| Wellness | $8M |

Ambulatory encounters contribute the highest total claim costs.

Urgent care accounts for approximately **13.1% of encounters** but contributes around **23% of total claim costs**.

This shows that encounter frequency and total claim costs do not always follow the same pattern.

**Key Finding:** Ambulatory services generate the highest total claim costs, while urgent care contributes a relatively large share of costs compared with its encounter volume.

**Business Importance:** Hospital management should consider both encounter frequency and cost when making financial decisions.

<img width="883" height="492" alt="image" src="https://github.com/user-attachments/assets/26dfc798-bc82-4b4f-9879-b9106489b21d" />


## 5. How Much of the Total Claim Cost Is Covered by Insurance Payers?

The financial dashboard reports:

| Financial KPI | Value |
|---|---:|
| Total Claim Cost | $101.51M |
| Total Payer Coverage | $31.10M |
| Difference Between Claim Cost and Coverage | $70.42M |
| Overall Coverage Rate | 30.63% |

Recorded payer coverage represents **30.63% of total claim costs**.

The remaining difference is approximately **$70.42 million**.

<img width="471" height="309" alt="Payer summary" src="https://github.com/user-attachments/assets/dbf62c40-aff7-4964-8b65-222a69f80e74" />


### Coverage Rate by Payer

| Insurance Payer | Coverage Rate |
|---|---:|
| Medicaid | 94.01% |
| Dual Eligible | 89.25% |
| Medicare | 77.96% |
| Blue Cross Blue Shield | 69.10% |

Other payer categories show considerably lower recorded coverage rates.

**Key Finding:** Insurance coverage differs significantly across payers, and recorded payer coverage is substantially lower than total claim costs.

**Business Importance:** Understanding these differences can help hospital management review insurance arrangements and improve financial monitoring.

**Note:** The difference between claim costs and payer coverage does not necessarily represent unpaid bills or financial losses.

<img width="882" height="490" alt="coverage Rate By Payer" src="https://github.com/user-attachments/assets/806c7715-83ba-4dd0-8d09-6acb8f7d8e52" />


## 6. Which Procedures Are Performed Most Frequently?

**Total Procedures: 47,701**

The dashboard identifies **163 distinct procedure descriptions**.

The most frequently recorded procedures include:

| Procedure | Approximate Frequency |
|---|---:|
| Health and Social Care Assessment | 4,600 |
| Hospice Care | 4,100 |
| Depression Screening | 3,600 |
| Substance Use Assessment | 2,900 |
| Renal Dialysis | 2,700 |

Health and social care assessments are the most frequently recorded procedures.

**Key Finding:** Assessments, screenings and care-related procedures account for a significant share of procedure activity.

<img width="882" height="493" alt="Most Frequent Procedure" src="https://github.com/user-attachments/assets/afda2065-5afd-437c-b76e-869ab39fe9f7" />


## 7. Which Procedures Have the Highest Average Base Costs?

**Average Procedure Base Cost: $2,212**

The procedures with the highest average base costs include:

| Procedure | Approximate Average Base Cost |
|---|---:|
| Admit to ICU | $206,260 |
| Coronary Artery Bypass Grafting | $47,000 |
| Lumpectomy of Breast | $29,000 |
| Hemodialysis | $29,000 |
| Biventricular Implantable Device Insertion | $27,000 |

ICU admission has the highest average base cost.

However, the reported ICU average is based on only **five procedure records**, so it should not be treated as the typical cost of all ICU admissions.

**Key Finding:** Some procedures have significantly higher average base costs than others.

**Business Importance:** Monitoring high-cost procedures can help management understand major cost differences and support budgeting decisions.

<img width="881" height="491" alt="Average Base Cost" src="https://github.com/user-attachments/assets/735daae4-ff0b-4235-9866-a639fb1eaf02" />


## 8. How Do Average Claim Costs Differ Across Insurance Payers?

**Overall Average Claim Cost: $3,639.68**

The payer financial summary shows differences in average claim costs.

Examples include:

| Payer | Approximate Average Claim Cost |
|---|---:|
| Medicaid | $6,205 |
| No Insurance | $5,593 |
| Anthem | $4,237 |

Medicaid has one of the highest average claim costs among the payer categories shown.

These differences may reflect the types of encounters and services associated with each payer group.

**Key Finding:** Average claim costs vary across insurance payers.

**Business Importance:** Comparing payer-level costs can help hospital management understand financial patterns and identify areas requiring further attention.

---

# Key Performance Indicators

The dashboard presents the following operational and financial KPIs:

| KPI | Value |
|---|---:|
| Total Encounters | 27,891 |
| Unique Patients | 974 |
| Average Claim Cost | $3,639.68 |
| Total Claim Cost | $101.51M |
| Total Payer Coverage | $31.10M |
| Coverage Rate | 30.63% |
| Encounters Over 24 Hours | 0.27% |
| Total Procedures | 47,701 |
| Distinct Procedure Descriptions | 163 |
| Average Procedure Base Cost | $2,212 |
| Procedures per Encounter | 1.71 |

---

# Business Recommendations

## Recommendation 1 — Improve Staffing and Resource Planning

Ambulatory and outpatient encounters account for approximately 67.5% of all hospital visits.

**Recommendation:** Hospital management should prioritise staffing, appointment scheduling and resources for these services.

**Expected Benefit:** Better patient flow, reduced pressure on busy services and improved use of hospital resources.

## Recommendation 2 — Strengthen Financial and Insurance Coverage Monitoring

 Total claim costs reached $101.51 million, while recorded payer coverage was $31.10 million, representing a coverage rate of 30.63%.

**Recommendation:** Management should review payer coverage patterns and investigate why some insurance categories show very low recorded coverage.

**Expected Benefit:** Better understanding of coverage differences and improved financial planning.

## Recommendation 3 — Monitor Procedure Frequency and High-Cost Services

 The hospital recorded 47,701 procedures, with significant differences in procedure frequency and average base costs.

**Recommendation:** Management should use procedure frequency to plan routine resources and review high-cost procedures when making budget decisions.

**Expected Benefit:** More effective resource allocation and better cost management.

---

# Data Quality and Reporting Considerations

The following factors are important when interpreting the analysis:

- Some encounter and procedure records have missing reason codes or descriptions.
- Encounter-duration calculations depend on valid start and end timestamps.
- The 2022 reporting period should be considered when interpreting yearly trends.
- Average costs based on a small number of procedures should be interpreted carefully.
- Recorded payer coverage should not be treated as confirmed payment received.

These considerations help ensure that the findings are interpreted appropriately.

---

# Conclusion

This project demonstrates how healthcare records can be transformed into useful operational and financial insights through Power BI.

The analysis shows that ambulatory and outpatient services account for most hospital encounters, while claim costs vary across encounter classes and insurance payers.

It also highlights the difference between recorded claim costs and payer coverage, as well as variations in procedure frequency and average base costs.

The findings provide a basis for improving staffing decisions, monitoring healthcare costs and supporting better resource planning.

The project strengthened my practical skills in **Power Query, DAX, data modelling, dashboard development and business analysis**.

---

**Project:** Healthcare Operations & Financial Intelligence Dashboard  
**Programme:** AnalystLab Africa — 
**Tool:** Microsoft Power BI  
**Focus:** Healthcare Operations | Financial Intelligence | Procedure Utilisation
