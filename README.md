
# Databricks Data Quality Framework

An enterprise-grade Data Quality Framework built on Databricks Community Edition
monitoring data quality across Enterprise Data Lake assets using 5 DQ dimensions.

## DQ Summary
- **Transactions Dataset:** 10,150 records, 21 checks
- **Customers Dataset:** 5,075 records, 19 checks
- **Total DQ Checks:** 40
- **Transactions Overall DQ Score:** 99.13%
- **Customers Overall DQ Score:** 98.3%
- **Checks Passed:** 31/40
- **Total Failed Records:** 3,690

## DQ Dimensions Covered
1. **Completeness** - Null value detection across all columns
2. **Uniqueness** - Duplicate record and key detection
3. **Validity** - Business rule and range validation
4. **Timeliness** - Future date and stale data detection
5. **Consistency** - Cross-column and referential integrity checks

## Dashboard Sections
1. KPI Cards - Overall DQ Scores, Check Pass Rate, Failed Records
2. DQ Scores by Dimension - Banking Transactions
3. DQ Scores by Dimension - Customer Master
4. Failed Records by DQ Dimension
5. Check Status Distribution (PASS/WARN/FAIL)
6. Top Failing Checks
7. Data Quality Alerts and Recommendations

## Key Insights
- Completeness is the highest risk dimension with 2,445 failed records
- Transactions achieve 99.13% overall DQ score
- Customer Master achieves 98.3% overall DQ score
- Framework automatically generates remediation recommendations

## Architecture
- Enterprise Data Lake simulation with injected DQ issues
- Batch data service monitoring with DQ checks and alerts
- Automated DQ scoring across 5 dimensions
- Executive drill-down dashboard for business and leadership

## Technologies
- Python, PySpark (Databricks)
- Pandas, NumPy
- Matplotlib (Dashboard Visualization)
- Databricks Community Edition
- GitHub Integration (Automated Commits)
