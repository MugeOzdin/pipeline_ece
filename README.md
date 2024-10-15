# pipeline_ece

The purpose of this project is primarily to collect and prepare available data for a political strategy consulting firm. We went through several steps: The first was to retrieve a dataset, so we chose the regional elections of 2010 in CSV format, as CSV is widely used and easily manageable. Once the data was collected, we decided to process it using a NiFi flow and read it into a Kafka topic. First, we downloaded Kafka from this link: https://www.apache.org/dyn/closer.cgi?path=/kafka/3.0.0/kafka_2.13-3.0.0.tgz. 

Then we installed it using the following commands:
