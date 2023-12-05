# Analysis on Doctors that are Stakeholders in Healthcare 
## Business Problem
Conflicts of interests can be created when doctors are also stakeholders in their healthcare company. We are analyzing the transparency of the Open Payments data.
### Python Scripts and Purposes
1. create.py - Creates the Google Cloud Storage Bucket, Google Cloud BigQuery Data Warehouse, and Creates the BigQuery Tables within the Data Warehouse
   - Done via Google Cloud libraries available in Python (works similarly to APIs)
2. extract.py - This step takes our folder of data (csv files), which was downloaded from (insert the website we got the data from) and puts all that data into our Google Cloud Storage Bucket.
3. transform_load.py - This script pulls the data from the Google Cloud Bucket, Transforms it/cleans it up so that it fits our data model, and then it is pushed into our data warehouse tables
## Data
(insert - Flow chart with files and how they are connected to our data warehouses)
# Tools and Technologies

This project utilizes a range of tools and technologies, primarily focused around Python and Google Cloud services. Below is a list of key tools and libraries used:

## Python

- **Description**: A high-level, interpreted programming language known for its ease of use and readability.
- **Usage**: The primary programming language used for writing the ETL scripts (`extract.py`, `transform_load.py`, `create.py`).

## Google Cloud

- **Description**: A suite of cloud computing services that runs on the same infrastructure that Google uses internally for its end-user products.
- **Usage**: Provides the cloud infrastructure for data storage (Google Cloud Storage) and data warehousing (Google Cloud BigQuery).

## Python Libraries

### Pandas

- **Description**: An open-source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools.
- **Usage**: Used for data manipulation and analysis.

### Numpy

- **Description**: A library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions.
- **Usage**: Used for handling numerical data and calculations.

### Google Cloud Libraries

- **Description**: Libraries provided by Google for interacting with Google Cloud services.
- **Usage**: Used to interact with Google Cloud Storage and Google Cloud BigQuery.

### OS

- **Description**: A standard Python library that provides a way of using operating system dependent functionality.
- **Usage**: Used for handling file and directory operations.

### BigQuery Libraries

- **Description**: Libraries specifically designed to interact with Google BigQuery, enabling SQL-like queries.
- **Usage**: Used to manage and query data in Google Cloud BigQuery.

This list is not exhaustive but covers the primary tools and libraries utilized in the ETL process.

# ETL Methodology

This document outlines the ETL (Extract, Transform, Load) process designed for handling data using Google Cloud services. The process is divided into three main steps:

## 1. Extracting the Data

The extraction process is handled by the `extract.py` script. This script is responsible for:

- Accessing a folder of data (CSV files).
- The data is sourced from [Data Source Website](insert-website-link-here).
- Uploading the data to the Google Cloud Storage Bucket.

## 2. Transforming the Data

Transformation of data occurs in the `transform_load.py` script, which:

- Retrieves data from the Google Cloud Storage Bucket.
- Performs necessary cleaning and transformations to align with the data model.

## 3. Loading the Data

The final step of the ETL process, also part of the `transform_load.py` script, involves:

- Loading the transformed data into the BigQuery Tables within the Google Cloud BigQuery Data Warehouse.

## Infrastructure Setup

The `create.py` script is used to set up the required infrastructure:

- Creates the Google Cloud Storage Bucket.
- Establishes the Google Cloud BigQuery Data Warehouse.
- Generates the BigQuery Tables within the Data Warehouse.
- This setup utilizes Google Cloud libraries in Python, functioning similarly to APIs.

## Diagram of the ETL Process

Below is a simple diagram illustrating the ETL process flow:


