### Technologies employed
1. Database Schema Design - https://lucid.co/
2. Google Cloud Platform Services - Google Storage , Google Compute Engine, Google BigQuery
3. Data Pipeline Tool - https://www.mage.ai/
4. Data Visualization Tool - Looker Studio

### Programming Languages
1. Python
2. SQL

### Data
Website : https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page
Data Dictionary : https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf

### Entity Relationship Diagram Design
We will be utilizing https://lucid.co/ to create a entity relationship diagram, to help us visualize and design the schema
of the database by representing tables, columns, and relationships between the tables.

![entityrd](https://user-images.githubusercontent.com/130780065/236612655-99720e51-6ae7-4da9-803b-3feb343ae9d8.JPG)


### Workflow
Afterwards, We will leverage google cloud tools to perform Data Warehousing, Data Analysis and also MAGE to perform ETL and Looker Studio to visaulize the data.
![workflow](https://user-images.githubusercontent.com/130780065/236613410-ba92d508-a4f3-4fc6-9d1d-5d576b492dfd.JPG)

The project workflow can be summarized as follows:
1. Store the raw Uber data files in Google Cloud Storage.
2. Create a Compute Instance to run Python scripts or Jupyter Notebooks for data exploration and processing.
3. Use the Mage Data Pipeline Tool to create data pipelines that extract data from Cloud Storage, transform it using Python scripts, and load the transformed data into BigQuery.
4. Analyze and visualize the data in BigQuery using SQL queries and Looker Studio to create interactive dashboards and reports.

### ETL Tree

![tree](https://user-images.githubusercontent.com/130780065/236613438-e0ddabf7-437e-489a-9128-7c9cb296a7cf.JPG)

### Visualization From Looker
![uber_visualize](https://user-images.githubusercontent.com/130780065/236613454-b5807de4-883d-4903-a2f8-6065a6eba8a4.JPG)

# Summary Report
### Introduction:
As an intern at Uber, I have been tasked with performing data analytics on Uber's ride data using various tools and technologies, including Google Cloud Platform (GCP) services, Python, and external tools like Mage Data Pipeline Tool and Looker Studio. The goal of this project is to gain insights into the ride data to improve operational efficiency, customer satisfaction, and strategic decision-making.

### Architecture
The architecture of the project consists of several components, each serving a specific purpose in the data analytics process. The components include GCP Storage, Compute Engine, BigQuery, Looker Studio, Mage Data Pipeline Tool, and the usage of APIs for data ingestion.

### Data Ingestion using API and Google Cloud Storage
To obtain Uber's ride data, we can utilize Google Storage's API to fetch ride details, such as timestamps, location coordinates, and ride status. This data can be ingested periodically and stored in Google Cloud Storage as raw files. Cloud Storage provides a scalable, durable, and cost-effective solution for storing and retrieving data in various file formats (CSV, JSON, Avro, Parquet, etc.).

### Data Exploration and Processing with Compute Engine
Google Compute Engine offers advanced virtual machines that can be used for running Python scripts or Jupyter Notebooks for data exploration, processing, and transformation. In this project, a Compute Instance is used to interact with the raw data stored in Cloud Storage and perform initial analysis and processing using Python libraries like Pandas and NumPy.

### Data Transformation using Mage Data Pipeline Tool
Mage is a data pipeline tool that can be employed for data extraction, transformation, and loading (ETL) tasks. It automates the process of extracting data from sources like Cloud Storage, transforming it using Python scripts, and loading it into BigQuery for further analysis. In this project, Mage is used to create data pipelines that run on a Compute Instance to process the Uber ride data and load the transformed data into BigQuery.

### Data Storage and Analysis with BigQuery
BigQuery is a fully-managed, serverless data warehouse that enables users to analyze large datasets in real-time using SQL. The transformed Uber ride data is stored in BigQuery, where complex queries can be performed for data analysis and visualization.

### Data Visualization with Looker Studio
Looker Studio is a powerful data analytics and visualization tool that integrates with BigQuery. It allows users to create interactive dashboards and reports to gain insights from the data stored in BigQuery, enabling data-driven decision-making at Uber.

### Conclusion
By leveraging modern data engineering techniques and Google Cloud Platform services, we have built a scalable and robust data analytics solution for Uber's ride data. This solution allows us to extract valuable insights and make informed decisions to improve operational efficiency, customer satisfaction, and strategic planning at Uber. The use of API for data ingestion, combined with Cloud Storage, Compute Engine, Mage Data Pipeline Tool, BigQuery, and Looker Studio, provides a comprehensive and flexible approach to data engineering and analytics in a cloud-native environment.
