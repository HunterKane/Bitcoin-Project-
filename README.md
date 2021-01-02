# Bitcoin Project 



## Project Description

In this project I ETL a massive bitcoin historical transaction dataset into an analytics schema. I transfer the raw source datasets from an S3 bucket I have set up: "s3n://udacity-dend-crypto/bitcoin-historical-data/" into another S3 bucket: "s3n://udacity-dend-crypto/analytics/". The analytics S3 bucket will store the files in parquet format and the tables will be set up based on the analytics schema. This data was prepared for an analytics team that is interested in learning more about historical bitcoin transaction volumes. The data was prepared into an analytics schema that could be easily queried to answer various time based questions like "which market sold a greater volume of bitcoin in a particular month?". I assume the analyst would be using Python and Spark to query the data, which was the reasoning for storing the data as parquet files on S3. 

### Source Data

File 1: Bitstamp minute by minute data in csv format. (~4million rows x 8 Columns)

File 2: Coinbase minute by minute data in json format. (~2million rows x 8 Columns). 

### Analytics Schema

![Schema](https://github.com/ridicholas/Udacity-Dend-Capstone/blob/master/Schema.png)

### Tools Used

My primary goal for this project was to get more exposure in using PySpark and the AWS EMR resource. These are the most useful tools for me as an analyst and data scientist so I focused exclusively on these tools. The entire project is written in a Jupyter Notebook file that should be run from an EMR resource.


