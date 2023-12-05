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
### Tool Key
- Storage 
- Scripts (create.py, extract.py, transform_load.py)
- Dimensional Model
- Visualization
## ETL Methodology

### 1. Extracting the Data
 
### 2. Transforming the Data

### 3. Loading the Data

