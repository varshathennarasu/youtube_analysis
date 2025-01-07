# YouTube Analytics Project

This project leverages AWS cloud services to securely manage, streamline, and analyze YouTube video data, focusing on video categories and trending metrics. By building a scalable data pipeline with AWS, I learned the key aspects of data engineering: data ingestion, transformation, and visualization, while using tools like SQL, Python, and AWS.

## Project Overview

The goal of this project is to automate the ingestion, transformation, and analysis of YouTube video data, providing valuable insights into the performance and trends of videos across different regions. The system is designed to scale as the volume of data increases and to process data efficiently using AWS services.

## Key Project Goals

- **Data Ingestion**: Build an automated mechanism to ingest raw data from external sources(Kaggle datatset).
- **ETL System**: Transform raw data into a structured format for analysis.
- **Data Lake**: Centralized repository in Amazon S3 to store raw and processed data.
- **Scalability**: Design a system that scales to handle large amounts of data.
- **Cloud Integration**: Use AWS services for data storage, processing, and querying.
- **Reporting**: Build a reporting and visualization dashboard to analyze the trends.

## AWS Services Used

- **Amazon S3**: Used for scalable storage of raw and processed data.
- **AWS IAM**: Manages secure access to AWS resources.
- **Amazon QuickSight**: Business intelligence service for visualizing YouTube data and trends.
- **AWS Glue**: Serverless ETL service to transform and prepare data for analytics.
- **AWS Lambda**: Automates tasks like data ingestion, processing, and transformation in a serverless environment.
- **AWS Athena**: Provides SQL querying capabilities for analyzing data stored in Amazon S3 without needing to load it.

## Dataset Used

This project uses a Kaggle dataset containing statistics on daily trending YouTube videos. The dataset includes the following attributes:

- **Video Information**: Title, Channel title, Publication time, Tags, Views, Likes, Dislikes, Description, Comment count.
- **Region-Specific Data**: Video category data differs by region, identified using `category_id`.

[Download YouTube Dataset from Kaggle](https://www.kaggle.com/datasets/datasnaek/youtube-new)

## Architecture Overview

1. **Data Ingestion**:
   - Raw data is ingested from external sources and stored in Amazon S3.
   
2. **Data Transformation**:
   - AWS Glue crawls and transforms the raw data into structured formats for analysis.
   - AWS Lambda functions automate data transformation and cleaning tasks.
   
3. **Data Storage**:
   - Processed data is stored in Amazon S3, serving as the central data lake.

4. **Data Querying**:
   - AWS Athena allows fast querying on the data stored in S3 using SQL.

5. **Reporting**:
   - Insights and reports are created using Amazon QuickSight, providing a visual representation of video performance and trends.

## What I Learned

1. **Cloud Data Engineering**:
   - This project allowed to me learn how to design and implement scalable, cloud-based data pipelines using AWS services like S3, Lambda, Glue, and Athena.
   
2. **ETL Process & Automation**:
   - I automated the ETL pipeline using AWS Glue and Lambda functions to transform and process raw data, ensuring an efficient workflow.
   
3. **SQL Querying & Data Analysis**:
   - Using AWS Athena, I learned how to write SQL queries to analyze large datasets stored in S3, enabling real-time data insights.
   
4. **Python Scripting**:
   - Python is used throughout the project for automation, data processing, and integration with AWS services like Lambda and Glue.

5. **Data Visualization & Reporting**:
   - The project uses Amazon QuickSight to create interactive dashboards, helping to visualize trends and analyze video metrics.

6. **Scalability**:
   - The architecture is designed to scale with the growing volume of data, ensuring future-proofing for larger datasets.

## Project Files
- **Lambda Functions**: Python scripts for automating data ingestion and transformation tasks.
- **Glue Jobs**: Scripts for defining ETL jobs and schema discovery.
- **SQL Queries**: Athena queries for data analysis.
- **QuickSight Dashboards**: Links to or images of visualizations based on the dataset.
