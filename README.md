# Spotify End-To-End ETL Data Engineering Project

### Intoduction
In this project we build an ETL(Extract, Transform, Load) pipeline using Spotify API on AWS. The pipeline will retrieve data from Spotify API, transform it to a desired format, and load into AWS S3(Data Storage).

### Project Components
- Integrating with Spotify API and extracting Data
- Deploying code on AWS Lambda for Data Extraction
- Adding trigger to run the extraction automatically
- Writing transformation function
- Building automated trigger on transformation function
- Store files on S3 properly
- Building Analytics Tables on data files using Glue and Athena

### Architecture
![Architecture Diagram](https://github.com/LalithaSpoorthy/Spotify-end-to-end-ETL-data-engineering/blob/main/Spotify-etl-data-architecture.png)

### About Dataset/API
This API contains information about music artist, albums and songs - [Spotify API](http://developer.spotify.com/documentation/)

### Services Used
1. **AWS S3 (Simple Storage Service):** Amazon S3 is a highly scalable oject storage service that can store and retrieve any amount of data from anywhere on the web. It is commonly used to store and distribute large media files, data backups and static website files.
   
2. **AWS Lambda:** AWS Lambda is a serverless computing service that lets you run your code without managing severs. You can use Lambda to run code in response to events like changes in S3, DynamoDB, or other AWS services.

3. **Cloud Watch:** Amazon CloudWatch is a monitoring service for AWS resources and the applications you run on them. You can use CloudWatch to collect and track metrics, collect and monitor log files, and set alarms.

4. **Glue Crawler:** AWS Glue Crawler is a fully managed service that automatically crawls your data sources, identifies data formats, infer schemas to create an AWS Glue Data Catalog.

5. **Data Catalog:** AWS Glue Data Catalog is a fully managed metadata repositiory that makes it easy to discover and manage data in AWS. You can use the Glue Data Catalog with other AWS services such as Athena.

6. **Amazon Athena:** Athena is an interactive query service that makes it easy to analyze data in Amazon S3 using standard SQL. You can use Athena to analyze data in your Glue Data Catalog or in other S3 buckets.
   

### Install Packages
```
pip install pandas
pip install numpy
pip install spotipy
```

### Project Execution Flow
Extract Data from API -> Lambda Trigger (every 1 hour) -> Run Extract code -> Store Raw Data -> Tigger Transform Function -> Transform Data and Load -> Query using Athena

