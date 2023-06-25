# -Real-time-stock-market-analysis-with-Apache-Kafka-and-AWS-for-improved-decision-making
This project demonstrates an end-to-end data engineering solution for processing real-time stock market data using Apache Kafka, Python, and various AWS services such as Amazon S3, AWS Glue, and Amazon Athena. The goal of this project is to collect, store, and analyze stock market data in real-time.

Technologies Used
1. Python: Programming language used for data processing and integration tasks.
2. Apache Kafka: Distributed streaming platform used for collecting and processing real-time stock market data.
3. Amazon Web Services (AWS): Cloud computing platform utilized for hosting and managing the project.
4. Amazon EC2: Elastic Compute Cloud instances are used to set up and run the Kafka server.
5. Amazon S3: Scalable object storage service employed for storing stock market data.
6. AWS Glue: Serverless data integration service utilized for crawling and cataloging the stock market data in a data lake.
7. Amazon Athena: Interactive query service used to analyze and query the data stored in the data lake.
8. SQL: Query language employed for retrieving and manipulating the stock market data.

Project Workflow
1. Data Ingestion: Real-time stock market data is fetched from a data source and fed into the Kafka server, running on an Amazon EC2 instance. Python scripts are used to handle data retrieval and Kafka message production.
2. Data Storage: The stock market data streamed through Kafka is stored in an Amazon S3 bucket, ensuring scalable and durable data storage. Each message is persisted as a separate file in the S3 bucket, facilitating efficient data retrieval.
3. Data Integration: AWS Glue is utilized to create a crawler that automatically discovers the stock market data files in the S3 bucket. The crawler catalogs the files, their schema, and other metadata, enabling easy data querying and analysis.
4. Data Catalog: AWS Glue's crawler populates the AWS Glue Data Catalog with the stock market data, making it accessible through the catalog's metadata tables. The data is organized and structured based on the discovered schema.
5. Data Analysis: Amazon Athena is employed to perform SQL-based queries on the stock market data stored in the data lake. Analysts can use SQL statements to retrieve specific data subsets, perform aggregations, and gain valuable insights into stock market trends.

![Architecture](https://github.com/mvmananvora/-Real-time-stock-market-analysis-with-Apache-Kafka-and-AWS-for-improved-decision-making/assets/64776101/62dab3e1-f15c-468e-9252-31e629bb3591)
