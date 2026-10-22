# Data Quality Audit with Python

## Overview
This project demonstrates how Python and pandas can be used to identify common data-quality issues, clean duplicate records, flag questionable values, and generate audit reports from a synthetic customer dataset.

## Skills Demonstrated
- Data inspection and profiling
- Missing-value analysis
- Duplicate record detection
- Customer ID validation
- Email-format validation
- Age-range validation
- Data cleaning and quality flags
- CSV reporting

## Dataset
The project uses eight fictional customer records created for practice. No real customer data is included.

## Audit Findings
The initial dataset contained 8 rows and 5 columns. The audit identified:
- 1 exact duplicate record
- 2 rows involved in duplicate customer IDs
- 1 missing age
- 1 blank name
- 1 invalid email format
- 1 age outside the assumed valid range of 0–120

After removing the exact duplicate, 7 rows remained. Other issues were flagged for review rather than automatically changed.

## Project Files
- `data_quality_audit.ipynb` — analysis and cleaning workflow
- `cleaned_customer_data.csv` — cleaned dataset with review flags
- `audit_summary.csv` — summary of audit findings

## Tools
Python, pandas, Google Colab, GitHub

## Limitations
Email validation checks format only; it does not verify whether an email address exists. The age range is an assumed business rule for this exercise. Duplicate customer IDs should be reviewed before deciding which record to retain.
