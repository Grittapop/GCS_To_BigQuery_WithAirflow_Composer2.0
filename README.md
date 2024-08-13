# GCS_To_BigQuery_WithAirflow_Composer2.0

## Introduction
This project is focused on executing end-to-end data engineering processes. It leverages a variety of technologies to manage, process, and analyze data effectively. The key tools and platforms used in this project include Python, SQL, MySQL, Google Cloud Platform (GCP), Cloud Storage, Cloud Composer, BigQuery, and Apache Airflow.

## Architecture

![gcp 2 0](https://github.com/user-attachments/assets/5d5fb376-56f5-43a8-a520-fcc401d568e1)

## Technologies 
- Python
- MySQL
- Cloud Storage
- Cloud Composer
- BigQuery
- Apache Airflow

## Getting Started
### 1. Create a Cloud Composer Environment
- Start by creating a Cloud Composer environment in Google Cloud Console.

### 2. Configure PyPi Packages
- Once the environment is created, go to **PyPi Packages**.
- Set the required packages as specified in the instructions.
- Click Save to apply the changes.

![Screenshot 2024-08-13 135238](https://github.com/user-attachments/assets/89c742f7-a390-4aa1-8825-2abda3e2aea1)
  

### 3. Create a MySQL Connection
- Navigate to the Cloud Composer page.
- Go to **Airflow**, then **Admin -> Connections**.
- Create a new connection (Create Connections) for MySQL, providing the necessary details.

![airflowsql](https://github.com/user-attachments/assets/a3c11f05-f487-407f-b8f6-73290c9be0e1)


### 4. Create BigQuery Dataset and Table
- Go to BigQuery.
- Create a new Dataset name **workshop**.
- Within this Dataset, create a new Table name **audible_data**.

### 5. Upload the bq_load.py File
- Go to the **DAGs** 
- Upload the **bq_load.py** file to the dags folder in Cloud Storage associated with your Cloud Composer environment.

![dag](https://github.com/user-attachments/assets/7c846fd5-9caf-4dce-b1f0-e987e1c16419)


### 6. Run the DAG in Airflow UI
- Go to Airflow UI.
- Wait for the DAG name bq_load to appear.
- Click on the DAG and then click Run to start execution.
