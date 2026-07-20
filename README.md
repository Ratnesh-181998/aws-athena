# AWS Athena
Amazon Athena is a serverless, interactive query service that allows you to analyze data directly in Amazon S3 using standard ANSI SQL. Because it is serverless, there is no infrastructure to manage or set up. You pay only for the amount of data scanned per query, making it highly cost-effective

- https://www.amazonaws.cn/en/athena/
- https://docs.aws.amazon.com/boto3/latest/reference/services/athena.html
- https://docs.aws.amazon.com/athena/latest/ug/when-should-i-use-ate.html
- https://docs.aws.amazon.com/athena/latest/ug/what-is.html
- https://docs.aws.amazon.com/athena/
- https://aws.amazon.com/athena/

---

# Key Features and CapabilitiesZero ETL:
- You do not need to move or load data into a proprietary database; it queries files directly where they live in S3.
- Powered by Open Source: Athena is built on the Trino (formerly Presto) distributed SQL engine and Apache Hive, allowing for fast, parallelized processing of massive datasets.
- Supported Formats: It can process unstructured, semi-structured, and structured data, including CSV, JSON, Parquet, ORC, and Avro.
- Federated Queries: Through Athena Query Federation, you can run SQL queries across multiple data sources beyond S3—such as Amazon DynamoDB, RDS, Redshift, and even external systems like Google BigQuery.
- BI & Notebook Integration: Athena seamlessly connects to Business Intelligence (BI) tools like Amazon QuickSight, Tableau, and Power BI, and integrates with Amazon SageMaker for machine learning workflows

---

# How It Works
- Storage:Your raw data lives in an S3 bucket.
- Metadata: You use the AWS Glue Data Catalog to define the schema and location of your data. This acts as a bridge so Athena understands how to interpret the files in S3.
- Query: You use the Athena console or API to write and run standard SQL queries, with results automatically exported back to an S3 bucket of your choice


---

