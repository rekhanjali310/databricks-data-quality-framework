# Databricks Data Quality Framework

An enterprise-grade Data Quality Framework built on Databricks Community Edition
monitoring data quality across Enterprise Data Lake assets using 5 DQ dimensions
across 2 datasets, 15,225 records, and 40 automated checks.

## DQ Summary
- **Transactions Dataset:** 10,150 records, 21 checks, **99.14% Overall DQ Score**
- **Customers Dataset:** 5,075 records, 19 checks, **98.27% Overall DQ Score**
- **Total DQ Checks:** 40
- **Checks Passed:** 77.5%
- **Total Failed Records:** 3,685

## Dashboard Visualizations
![DQ Framework Dashboard](https://raw.githubusercontent.com/rekhanjali310/databricks-data-quality-framework/main/dq_dashboard.png)

## DQ Dimensions Covered
1. **Completeness** — Null value detection across all columns
2. **Uniqueness** — Duplicate record and primary key detection
3. **Validity** — Business rule and range validation
4. **Timeliness** — Future date and stale data detection
5. **Consistency** — Cross-column and referential integrity checks

## Dashboard Sections
1. **KPI Cards** — Transactions DQ Score, Customers DQ Score, Checks Passed, Failed Records
2. **DQ Scores by Dimension** — Banking Transactions across 5 dimensions
3. **DQ Scores by Dimension** — Customer Master across 5 dimensions
4. **Failed Records by DQ Dimension** — Completeness highest risk at 2,395 failed
5. **Check Status Distribution** — PASS 77.5%, WARN 20.4%, FAIL 2.5%
6. **Top Failing Checks** — Age range, KYC status, email completeness
7. **Data Quality Alerts and Recommendations** — Automated remediation guidance

## Key Insights
| Dimension | Transactions | Customers | Status |
|---|---|---|---|
| Completeness | 98.84% | 98.07% | PASS |
| Uniqueness | 98.56% | 97.34% | PASS |
| Validity | 100.00% | 99.44% | PASS |
| Timeliness | 99.51% | N/A | PASS |
| Consistency | 98.77% | 98.24% | PASS |
| **Overall** | **99.14%** | **98.27%** | **PASS** |

## Architecture
- Enterprise Data Lake simulation with injected DQ issues
- Batch data service monitoring with automated DQ checks and alerts
- DQ scoring across 5 dimensions with drill-down visibility
- Executive dashboard for business and leadership reporting
- GitHub integrated via Databricks Git folders

## Technologies
- Python, Pandas, NumPy
- Matplotlib (Custom Dashboard)
- Databricks Community Edition
- GitHub Integration (Automated Commits)
