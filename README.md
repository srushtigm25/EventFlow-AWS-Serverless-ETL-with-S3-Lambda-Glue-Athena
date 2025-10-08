# EventFlow-AWS-Serverless-ETL-with-S3-Lambda-Glue-Athena
An event-driven ETL on AWS using fully managed services: S3, Lambda, Glue (Job + Crawler + Catalog) and Athena.

This repo is an implementation of an AWS ETL pipeline: ingest raw files, trigger a transformation job automatically, catalog the schema, and query with SQL—no servers to manage.

🧰 Tech Stack - 

Amazon S3 – raw & curated data lakes

AWS Lambda – event trigger + job launcher/light transforms

AWS Glue – ETL job (Spark/PySpark), Crawler, Data Catalog

Amazon Athena – interactive SQL on curated data

IAM – least-privilege roles & policies

🧪 Data Flow Test - 

Drop a sample file into s3://<prefix>-eventflow-raw/raw/2025-10-07/…

Confirm: Lambda logs show StartJobRun; Glue Job runs to completion

Run crawler → tables update

Query in Athena

References - 

This project implements the strategy described in:

https://youtu.be/yHHCV3Q13Fo?si=zwAFB3rEdAbqDha7



