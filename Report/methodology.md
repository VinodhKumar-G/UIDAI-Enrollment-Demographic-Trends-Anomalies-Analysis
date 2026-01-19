# Methodology
This document describes the analytical approach used to study Aadhaar enrolment and demographic update data for identifying trends and anomalies.


## 1. Data Sources

The analysis is based on two UIDAI datasets:
- Aadhaar Enrolment Data (age-wise enrolments by date and district)
- Aadhaar Demographic Update Data (age-wise demographic updates by date and district)

Both datasets are provided at a granular level and contain temporal and geographic attributes.



## 2. Data Cleaning and Preprocessing

- Date fields were standardized to a consistent day-first format.
- Invalid or malformed dates were safely handled to prevent processing errors.
- Missing numeric values in age-wise counts were replaced with zero.
- New features such as monthly time periods and total enrolments/updates were derived.


## 3. Data Aggregation

To enable effective analysis:
- Raw records were aggregated at a **monthly and district level**.
- Age-wise enrolments and demographic updates were summed to create meaningful trend indicators.

This aggregation reduces noise while preserving all relevant information.



## 4. Trend Analysis

Trend analysis was performed to:
- Study changes in enrolment and update volumes over time
- Compare enrolment growth versus demographic update growth
- Understand age-group participation patterns

Line charts and aggregated summaries were used for interpretation.


## 5. Anomaly Detection

Anomalies were identified using a statistical threshold-based approach:
- Mean and standard deviation were calculated for update volumes
- Values exceeding the defined threshold were flagged as anomalies

Anomaly detection was performed at both national and district levels to capture localized irregularities.



## 6. Interpretation and Insights

All detected trends and anomalies were interpreted in the context of:
- Migration patterns
- Digital adoption
- Administrative and seasonal factors

The methodology emphasizes explainability, transparency, and practical relevance.
