# Spotify End-To-End ETL Data Engineering Project

### Intoduction
In this project we build an ETL(Extract, Transform, Load) pipeline using Spotify API on AWS. The pipeline will retrieve data from Spotify API, transform it to a desired format, and load into AWS S3(Data Storage).

### Architecture
![Architecture Diagram](https://github.com/LalithaSpoorthy/Spotify-end-to-end-ETL-data-engineering/blob/main/Spotify-etl-data-architecture.png)

### Services Used
1. **AWS S3 (Simple Storage Service):** Amazon S3 is a highly scalable oject storage service that can store and retrieve any amount of data from anywhere on the web. It is commonly used to store and distribute large media files, data backups and static website files.
   
2. **AWS Lambda:** AWS Lambda is a serverless computing service that lets you run your code without managing severs. You can use Lambda to run code in response to events like changes in S3, DynamoDB, or other AWS services.

3. **Cloud Watch:** Amazon CloudWatch is a monitoring service for AWS resources and the applications you run on them. You can use CloudWatch to collect and track metrics, collect and monitor log files, and set alarms.

4. **Glue Crawler:** AWS Glue Crawler is a fully managed service that automatically crawls your data sources, identifies data formats 
