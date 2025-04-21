
# Uber ETL Pipeline and Analytics 

## Introduction

The goal of this project is to perform data analytics on Uber data using various tools and technologies, including GCP Storage, Python, Compute Instance, Mage Data Pipeline Tool, BigQuery, and Looker Studio.

## Architecture

<img src="uber ETL Pipeline data engineering\architecture.jpg">

## Technology Used
- **Programming Language**: Python
- **Google Cloud Platform**:
  1. Google Storage
  2. Compute Instance
  3. BigQuery
  4. Looker Studio
- **Modern Data Pipeline Tool**: [Mage.ai](https://www.mage.ai/)

## Installation Process

To set up and run this project on your local environment, follow these steps:

### Prerequisites:
- Python 3.x
- Google Cloud Platform (GCP) account
- Mage.ai account
- BigQuery setup in your GCP console
- Looker Studio access

### Steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/kamalesh-29/Uber-ETL-Pipeline-Data-Engineering.git
   cd uber-etl-pipeline-data-engineering-project
   ```

2. **Set Up Python Environment:**
   - Create a virtual environment (optional but recommended):
     ```bash
     python -m venv venv
     source venv/bin/activate  # For Linux/MacOS
     .\venv\Scripts\activate  # For Windows
     ```

3. **Install Required Libraries:**
   - Install necessary Python libraries:
     ```bash
     pip install -r requirements.txt
     ```

4. **Set Up Google Cloud Platform (GCP):**
   - Ensure you have a GCP account and have configured `gcloud` CLI on your machine.
   - Set up **Google Storage**, **Compute Instance**, and **BigQuery** in your GCP console.
   - Set up **Looker Studio** for visualizations.

5. **Run the Mage Data Pipeline Tool:**
   - Install Mage.ai if you haven't already:
     ```bash
     pip install mage-ai
     ```
   - Run the Mage tool and configure it to integrate with your project:
     ```bash
     mage init
     mage start
     ```

6. **Upload Data to BigQuery:**
   - Upload the `uber_data.csv` dataset to BigQuery.
   - You can follow the steps to load CSV data from Google Cloud Storage into BigQuery.

7. **Run the ETL Pipeline:**
   - Execute the Python scripts or Jupyter notebooks to run the ETL pipeline:
     ```bash
     python Uber_Data_Pipeline.py
     ```

8. **Analyze the Data Using Looker Studio:**
   - Connect your BigQuery instance to Looker Studio and create dashboards for data visualization.

## Dataset Used

- **TLC Trip Record Data**: The dataset includes fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts.

Here is the dataset used in the project:  
[Uber Data CSV](https://github.com/darshilparmar/uber-etl-pipeline-data-engineering-project/blob/main/data/uber_data.csv)

More info about the dataset can be found here:  
1. [Website](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)  
2. [Data Dictionary](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf)

## Data Model

<img src="uber ETL Pipeline data engineering\data_model.jpeg">

