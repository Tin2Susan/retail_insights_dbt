# Retail Insights Pipeline using dbt + BigQuery

This project showcases an end-to-end data pipeline for generating actionable retail insights from Instacart's open dataset using modern data tools like **dbt**, **SQL**, and **BigQuery**.

## Project Overview

The goal is to build a modern analytics pipeline that:
- Loads raw retail data into BigQuery
- Cleans and transforms it using **dbt**
- Builds layered data models (staging → intermediate → marts)
- Produces insights such as customer behavior, product trends, and order patterns
- Can be extended to dashboards or predictive models later

##  Tech Stack

| Tool        | Purpose                          |
|-------------|----------------------------------|
| **dbt**     | Data modeling and transformation |
| **BigQuery**| Cloud data warehouse             |
| **SQL**     | Data analysis and transformation |
| **GitHub**  | Version control                  |
|             | Looker Studio or Power BI        | Dashboards (to be added later) |

## Project Structure


## Sample Insights (Planned)
- Top-selling products and aisles
- Order volume trends by hour/day
- Repeat purchase behavior
- Average basket size per user
- Product affinity (users who bought X also bought Y)

## Dataset

Source: [Instacart Market Basket Analysis](https://www.kaggle.com/datasets/psparks/instacart-market-basket-analysis)

- ~3 million orders
- 50,000 unique products
- User–product order history

## Data Modeling Approach

Using **dbt's layered architecture**:
- `staging/`: Clean, rename, and standardize raw tables
- `intermediate/`: Join and enrich data
- `marts/`: Business-ready models for KPIs and reporting

## Current Progress

- [x] GitHub + dbt project initialized  
- [x] Folder structure created  
- [ ] Data uploaded to BigQuery  
- [ ] dbt models created and tested  
- [ ] dbt docs generated  
- [ ] Dashboards (planned)

# Install dbt for BigQuery
pip install dbt-bigquery

# Run models
dbt run
