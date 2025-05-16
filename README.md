# p2-project-team1

# Global Sales ETL Pipeline – GCP Project

## Project Objective
Build a scalable ETL pipeline to process, clean, and analyze sales data from 8 countries, and deliver actionable insights via dashboards and forecasting using Google Cloud services.

## Countries & Data Sources
- **India**: SQL Server
- **Japan**: CSV (Cloud Storage)
- **Norway**: PostgreSQL (AlloyDB)
- **Sri Lanka**: JSON (Cloud Storage)
- **Hong Kong**: Excel File
- **Oman, Germany, Qatar**: MySQL Instances

## Categories & Products
- **Categories**: T-Shirts, Jeans, Shoes, Smartphones, Perfumes, Water Bottles
- **Each category**: 6 unique products
- **Currency normalization**: All prices are converted to INR

## Architecture Diagram
![ETL Pipeline](diagrams/etl-pipeline-architecture.png)

## ETL Pipeline Steps
1. **Extract**: Load data from various formats and sources
2. **Transform**:
   - Convert currencies to INR
   - Remove nulls and invalid entries
   - Add computed fields (amount, tax, etc.)
3. **Load**: Cleaned, enriched data is stored in **BigQuery**

## Technologies Used
- **Google Cloud Platform (GCP)**
  - Cloud Storage
  - Dataproc (PySpark)
  - BigQuery
  - Looker Studio (Dashboards)
- PySpark, pandas, SQL

## Stakeholder Reports
- **A. CSV report** – Total quantity and amount sold
- **B. Visual dashboard** – Category-wise & Country-wise graphs
- **C. Tax Analysis** – 5% tax per sale, visualized per country
- **D. Misc. Charts** – Trend, Forecasting, Product performance

## Forecasting
Using BigQuery ML to forecast next month's sales and guide production planning.

## Folder Overview
| Folder        | Contents |
|---------------|----------|
| `data/`       | Sample input files per country |
| `scripts/`    | ETL code & utilities |
| `diagrams/`   | Project architecture |
| `dashboards/` | Stakeholder CSVs, Looker links, chart images |

## License
MIT License

## Author
Batch One | Revature Portfolio Project – GCP Data Process Engineer

