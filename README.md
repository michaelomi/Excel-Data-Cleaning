# Excel Data Cleaning Project

## 📄 Overview
This project involved cleaning and preparing a raw dataset in Excel for further analysis. The dataset contained customer orders, region details, and marketing information. The goal was to identify and address data quality issues, improve consistency, and document any limitations.

## 🧹 Cleaning Objectives
- Fix formatting issues
- Handle missing or inconsistent data
- Standardize text and numerical values
- Ensure proper data types for analysis

## 📊 Dataset
- `Orders` Table: ~20,000 rows of customer orders and transaction details
- `Region` Table: Country and region codes


## 🛠️ Issues Log & Resolutions

| Table  | Column(s)                      | Issue Description                                                | Row Count | Magnitude | Solvable | Resolution                                                      |
|--------|--------------------------------|------------------------------------------------------------------|-----------|-----------|----------|-----------------------------------------------------------------|
| Region | REGION_CODE                    | Some values not abbreviated, blanks, incorrect codes            | 9         | 4.69%     | Yes      | Assigned correct region country codes                           |
| Orders | All                            | Inconsistent text sizes                                          | -         | -         | Yes      | Formatted all font size to 12                                   |
| Orders | USER_ID, ORDER_ID, PRODUCT_ID  | Inappropriate data types                                         | -         | -         | Yes      | Corrected all column data types                                 |
| Orders | ORDER_ID                       | Duplicate values                                                 | 145       | 0.66%     | No       | Ignored due to low magnitude                                    |
| Orders | PURCHASE_TS                    | Inconsistent date formats                                        | 10        | 0.05%     | Yes      | Unified date format across dataset                              |
| Orders | PURCHASE_TS                    | Missing dates                                                    | 1         | 0.00%     | No       | Left as-is, sent to sales for further validation                |
| Orders | PRODUCT_NAME                   | Incorrect spelling                                               | 4662      | 21.33%    | Yes      | Corrected to "27inches 4K gaming monitor"                       |
| Orders | USD_PRICE                      | Missing or zero values                                           | 34        | 0.16%     | No       | Alerted sales team about missing data                           |
| Orders | MARKETING_CHANNEL              | Blank values                                                     | 83        | 0.38%     | Yes      | Categorized as "unknown"                                       |
| Orders | MARKETING_CHANNEL              | "unknown" entries                                                | 47        | 0.22%     | No       | Unaltered, pending validation from marketing team               |
| Orders | ACCOUNT_CREATION_METHOD        | Blank values                                                     | 83        | 0.38%     | Yes      | Categorized as "unknown"                                       |
| Orders | ACCOUNT_CREATION_METHOD        | "unknown" entries                                                | 743       | 3.40%     | No       | Unaltered, awaiting stakeholder input                           |
| Orders | COUNTRY_CODE                   | Blank values                                                     | 37        | 0.17%     | No       | Unaltered, needs stakeholder validation                         |
| Orders | SHIP_TS                        | Shipping date earlier than purchase date                        | 2003      | 9.17%     | No       | Left for further revalidation in shipping analysis              |


## 📁 Files
- `raw_data.xlsx` – Original dataset (anonymized if needed)
- `cleaned_data.xlsx` – Cleaned version with corrections
- `issues_log.csv` – Tabular format of the issues above
- `README.md` – This documentation


## 🧠 Notes
- Certain unresolved issues were left for business teams to validate due to external dependencies.
- The cleaned dataset can now be confidently used for further analysis or dashboard reporting.


## 📬 Contact
For any questions or suggestions, feel free to open an issue or contact me.
mailto:omimichael713@gmail.com
