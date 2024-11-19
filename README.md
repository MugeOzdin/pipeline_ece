# pipeline_ece

Introduction

The purpose of this project is to collect, process, and orchestrate data for a political strategy consulting firm. This involves building a data pipeline to handle datasets and ensure the automantion of data processing tasks.

The project consists of three main parts:
1. Data Collection
2. Data Processing (Formatting, Cleaning, etc.)
3. Orchestration and Automation of the Data Pipeline

Data Collection

The initial step involved retrieving a dataset. The regional elections data from 2010, provided in CSV format, was selected. CSV files are chosen for their simplicity and ease of management. Source: https://www.data.gouv.fr/fr/reuses/50-1-dis-moi-ou-tu-habites-je-te-dirai-pour-qui-tu-votes/

Data Processing (Formatting, Cleaning, etc)
After the data was collected, a consolidated dataset was created by combining the outputs of various data processing batches to produce a final file.

Several operations were performed primarily using PySpark, including:
1. Removing duplicates.
2. Handling symbols.
3. Processing dates.
4. Adding new columns through feature engineering. 
5. Calculating aggregates.

Technical Steps and Tools
1. File Selection: A suitable dataset was chosen.
2. Kafka topic creation: A Kafka topic was defined to manage real-time data streams.
3. Nifi flow creation: A data flow was developed using Apache Nifi to manage data ingestion and transformation.
4. Nifi and Nifi Registry ingestion: Nifi was linked to Nifi Registry to enable version control of data flows.
5. Bucket setup with Nifi Registry: A storage bucket was created, and the required authentification token was retrieved.
6. Handling large files: The file size exceeded Kafka's processing limits, and alternative methods were implemented for data handling.
7. Airflow orchestration: The data pipeline was orchedtrated and automated using Apache Airflow to ensure efficient and repeatable processes.


