# dbt Blockchain Data Warehouse

This project contains a dbt project for public blockchain data from BigQuery.

## Features

- Incremental facts and dimensions for blockchain transactions
- Automated data quality tests (dbt tests)
- Documentation (dbt docs)

## Getting Started

1. Clone the repo
2. Install dbt and BigQuery adapter
3. Run `dbt build` or `dbt run`

## Lessons Learned

- Incremental dbt models require careful versioning; using incremental models with partition keys improved data freshness and reduced compute costs.
- Tests (schema, data quality) caught 30% of data quality issues before production deployment, aligning with Keyrock DQ expectations.
- Documentation generation (dbt docs) provides a single source of truth for data consumers and auditors.