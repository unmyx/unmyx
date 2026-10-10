# Daniel Đuriš | Data Engineering & Analytics

Data Engineer and Analyst focused on **Python, SQL, ETL pipelines and automation**. I turn messy data and repetitive manual reporting into clean, validated, automated workflows.

I have 1 year of professional experience as a Data Analyst at Kyndryl (SQL on MySQL, Python automation, SAP S/4HANA data, Power BI dashboards). The projects below are self-directed builds that show how I design, test and document data workflows.

> All projects use synthetic or public data. None is client work.

## Core Skills

- **Languages:** Python, SQL, Java
- **Data Engineering:** ETL/ELT pipelines, API ingestion, data migration, incremental and idempotent loading, dbt
- **Databases:** PostgreSQL, MySQL
- **Data Quality:** validation, reconciliation, deduplication, exception reporting, automated testing
- **Analytics:** pandas, SQL analytics, statistical analysis, KPI reporting, A/B testing
- **Reporting:** Excel automation, Power BI (DAX), Tableau
- **Engineering Practices:** pytest, CI (GitHub Actions), Docker, structured logging, reproducible workflows, Git

## Featured Projects

| # | Project | What it does | Highlights |
|---|---------|--------------|------------|
| 1 | [Excel Reconciliation & QA System](https://github.com/unmyx/excel-reconciliation-qa-system) | Reconciles orders vs payments exports into a 10-tab review workbook | 7,500 orders / 7,994 payments, row-level traceability, 170 tests |
| 2 | [Business Reporting Pipeline](https://github.com/unmyx/business-reporting-pipeline) | Weekly reporting stack: PostgreSQL warehouse, Excel report, Power BI dashboard | 18 validation checks, EUR normalization, 4-page dashboard, 57 tests |
| 3 | [Automated Data Collection Pipeline](https://github.com/unmyx/automated-data-collection-pipeline) | Hourly weather API collection into PostgreSQL | Idempotent re-runs, retries, scheduler, 576 tests, 95.8% coverage |
| 4 | [Legacy Customer Data Migration](https://github.com/unmyx/legacy-customer-data-migration-pipeline) | Migrates messy CSV and Excel exports into normalized PostgreSQL | 448 rows to 306 customers, field-level provenance, 385 tests |
| 5 | [Production-Style ETL Pipeline](https://github.com/unmyx/production-etl-pipeline) | REST API and CSV into a PostgreSQL star schema with SQL views | Revenue reconciled exactly, rerun-safe loads, 0 orphan keys |
| 6 | [E-commerce Customer & Revenue Analytics](https://github.com/unmyx/ecommerce-customer-revenue-analytics) | SQL marts and Python analysis of revenue, RFM segments, cohorts and campaigns | 84,263 orders, A/B tests with FDR control, 215 tests |
| 7 | [FleetOps Game Analytics](https://github.com/unmyx/fleetops-analytics) | Game telemetry platform: PostgreSQL, dbt, statistics and a Tableau dashboard | 13M rows, 64 dbt models, 137 dbt tests, 27 SQL queries |

### Project details

**1. Excel Reconciliation & QA System**: handles split payments, duplicates, and currency and status mismatches. Bad rows are quarantined with a reason instead of being dropped.
*Python, pandas, openpyxl, pytest*

**2. Business Reporting Pipeline**: Python loads CSV and exchange-rate API data through raw, staging and reporting layers, then generates an 8-sheet Excel report and feeds a Power BI model.
*Python, PostgreSQL, SQL, Power BI, DAX, Docker*

**3. Automated Data Collection Pipeline**: incremental collection with watermarks, four validation layers, advisory-lock overlap protection and a full run audit trail.
*Python, httpx, SQLAlchemy, Alembic, PostgreSQL, Docker*

**4. Legacy Customer Data Migration**: config-driven mapping, E.164 phone normalization, deterministic duplicate merging, review queue for uncertain matches, transactional loading and audit reports.
*Python, pandas, PostgreSQL, phonenumbers*

**5. Production-Style ETL Pipeline**: paginated extraction, nested JSON flattening, validation that blocks bad loads, reconciliation inside the load transaction and per-run metadata.
*Python, pandas, PostgreSQL, SQL, Docker Compose*

**6. E-commerce Customer & Revenue Analytics**: RFM segmentation, cohort retention, campaign evaluation (Welch t-test, bootstrap, FDR control) and 18 dashboard-ready datasets with DAX measures.
*Python, SQL, PostgreSQL, statistics, Power BI kit*

**7. FleetOps Game Analytics**: deterministic synthetic telemetry for a fictional naval game, dbt layers from staging to marts, three validation layers, advanced SQL, statistical analysis (confidence intervals, power analysis, A/B experiment) and a completed 8-view Tableau balance dashboard.
*Python, PostgreSQL, dbt, SQL, Tableau, SciPy*

## How I Approach Data Problems

- **Validate** data instead of assuming it is correct.
- **Make workflows repeatable**, so the same task is not done by hand every week.
- **Handle duplicates, missing records and inconsistent sources explicitly.**
- **Test and reconcile** so results can be verified.
- **Document** setup, assumptions and business rules.

Each repository includes setup instructions, documentation and verified results.

## Contact

Open to freelance data engineering and automation work.

- Upwork: [My Upwork profile](https://www.upwork.com/freelancers/~01c676dbf7250a69c1)
- Email: [depduris@gmail.com](mailto:depduris@gmail.com)
