# Analysis of Doctors as Stakeholders in Healthcare 

## Business Problem
This analysis focuses on potential conflicts of interest arising when doctors hold stakeholder positions in their healthcare companies. We aim to assess the transparency of Open Payments data in this context.

## Data Overview
(Insert a flow chart here to illustrate how files are connected to our data warehouses.)

## ETL Methodology
Our ETL (Extract, Transform, Load) process, leveraging Google Cloud services, is divided into three primary steps:

### 1. Extracting the Data
Handled by `extract.py`, this script:
- Accesses a folder of data (CSV files) sourced from [Data Source Website](insert-website-link-here).
- Uploads the data to the Google Cloud Storage Bucket.

### 2. Transforming the Data
The `transform_load.py` script:
- Retrieves data from the Google Cloud Storage Bucket.
- Cleans and transforms the data to align with our data model.

### 3. Loading the Data
Conducted through `transform_load.py`, this final step:
- Loads the transformed data into the BigQuery Tables within the Google Cloud BigQuery Data Warehouse.

### Python Scripts and Their Functions
1. `create.py` - Sets up the Google Cloud Storage Bucket, Google Cloud BigQuery Data Warehouse, and the BigQuery Tables within the Data Warehouse.
2. `extract.py` - Processes and uploads the data (csv files) into the Google Cloud Storage Bucket.
3. `transform_load.py` - Transforms and loads the cleaned data into the data warehouse tables.

### Infrastructure Setup
The `create.py` script establishes the necessary infrastructure:
- Creates the Google Cloud Storage Bucket and the Google Cloud BigQuery Data Warehouse.
- Generates the BigQuery Tables within the Data Warehouse.
- Utilizes Google Cloud libraries in Python, akin to API functions.

### ETL Process Diagram
(Insert ETL process flow diagram here.)

## Tools and Technologies
Our project extensively uses Python and Google Cloud services. Below is a breakdown of the key tools and libraries:

### Python
- **Description**: An intuitive, high-level programming language.
- **Usage**: Primary language for writing our ETL scripts.

### Google Cloud
- **Description**: A comprehensive suite of cloud computing services.
- **Usage**: Provides infrastructure for data storage (Google Cloud Storage) and data warehousing (Google Cloud BigQuery).

### Python Libraries
#### Pandas
- **Description**: A powerful data manipulation and analysis tool.
- **Usage**: Employed for complex data operations.

#### Numpy
- **Description**: Enhances Python with support for large numerical arrays.
- **Usage**: Crucial for numerical data handling.

#### Google Cloud Libraries
- **Description**: Facilitates interaction with Google Cloud services.
- **Usage**: Integral for operations with Google Cloud Storage and BigQuery.

#### OS
- **Description**: Enables operating system dependent functionalities.
- **Usage**: Manages file and directory operations.

#### BigQuery Libraries
- **Description**: Specialized for querying Google BigQuery.
- **Usage**: Manages and queries data within Google Cloud BigQuery.

(Note: This is a representative list, highlighting primary tools and libraries used in the ETL process.)
