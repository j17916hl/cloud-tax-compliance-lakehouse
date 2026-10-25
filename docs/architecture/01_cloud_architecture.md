# Cloud Architecture

## Business Objective

Provide a scalable cloud-native platform for tax compliance analytics, data governance, and reporting.

---

## Source Systems

- W2 Data
- 1099 Data
- PIT Returns
- Payment Data
- Taxpayer Master
- Employer Registry

---

## Cloud Architecture

Source Systems

↓

Azure Data Lake Storage

(Bronze Layer)

↓

Databricks Processing

(Silver Layer)

↓

Business Data Products

(Gold Layer)

↓

Power BI

↓

Business Users

---

## Bronze Layer

Purpose:
Store raw source information exactly as received.

Examples:
- raw_w2
- raw_1099
- raw_returns
- raw_payments

---

## Silver Layer

Purpose:
Validated and curated data.

Examples:
- taxpayers
- employers
- returns
- payments

---

## Gold Layer

Purpose:
Business-ready outputs.

Examples:
- nonfiler_cases
- underreporting_cases
- revenue_metrics
- compliance_dashboard_metrics

---

## Orchestration

Apache Airflow

- Ingestion DAG
- Curation DAG
- Validation DAG
- Anomaly Detection DAG
- Case Creation DAG

---

## Governance

- Data Dictionary
- Data Lineage
- Quality Rules
- Metadata Documentation

---

## Future Enhancements

- Azure Synapse
- Power BI
- CI/CD
- Monitoring
- Observability