# GA4 SQL Marketing Analytics Portfolio

This project analyzes Google Analytics data using SQL in BigQuery to extract meaningful marketing insights. It's part of my data analytics portfolio and demonstrates how SQL can help answer business questions about user behavior, marketing channel performance, and revenue.

## Project Goals

- Segment users by device and marketing channel
- Calculate session-to-transaction conversion rates
- Visualize revenue by marketing campaign

## Dataset

- **Source**: [Google Analytics Sample Dataset (BigQuery Public Data)](https://console.cloud.google.com/marketplace/product/bigquery-public-data/google_analytics_sample)
- **Table**: `bigquery-public-data.google_analytics_sample.ga_sessions_*`

## Tools Used

- **SQL** (BigQuery)
- **Google Cloud Platform**
- (Optional) **Tableau / Looker Studio** for visualizations

## Key Queries

- Revenue by marketing channel
- Conversion rate by device
- Revenue by campaign

See the [`queries/`](./queries) folder for SQL scripts.

## Sample Output (Optional)

![Revenue by Channel](./visuals/revenue_by_channel.png)

## Learnings

- Navigating nested fields in BigQuery (e.g., `totals`, `device`, `trafficSource`)
- Aggregating and filtering transaction data
- Calculating conversion metrics from raw session data

## Notes

- Revenue is stored in micros; divide by 1,000,000 to convert to USD
- Use `SAFE_DIVIDE` to avoid division by zero

---

## About Me

I've completed an MBA in Data Analytics and building a portfolio that blends marketing and data insights. Connect with me on [LinkedIn](www.linkedin.com/in/zoecollinst).
