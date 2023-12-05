# Stock Market Data Analysis Using Kafka and AWS

## Overview
This project leverages kafka's fast and real time processing system and build a pipeline encompassing various AWS services and process stock market's simulated real time data, which is analyzed to produce desired outcomes.


## Project Goals
- Data Ingestion — Build a mechanism to ingest data from python script
- ETL System — Reading the data in csv format, transforming this data into json
- Data lake — Centralized storage system for data received from kafka messaging load
- Analysis — Store processed data in a database so that necessary analysis can be deduced from it 


## Steps Performed
1. Loaded data from csv file into kafka, after tranforming it into chunks of json files
2. Hosted kafka on AWS EC2 server and ingested data in json format from local python scipt
3. Stored data on S3 bucket from kafka for further data processing
4. Build a glue crawler on this S3 bucket and loaded this data into glue database catalog
5. Ran SQL queries on this database catalog in Athena to get the desired output



## Architecture Diagram

![Architecture](https://github.com/skyrim23/stock-market-data-analysis-kafka-aws/assets/27095356/8f31746c-3ef2-49b0-b200-bfb7856a3834)
