# ETL Weather Airflow Pipeline

## Overview

This project implements an **End-to-End ETL (Extract, Transform, Load) Pipeline** to retrieve, process, and store weather data from a public API into a PostgreSQL database. Using cutting-edge tools like **Apache Airflow**, **Docker**, and **Astronomer**, the pipeline delivers data-driven decision-making for weather analysis and forecasting.

## Key Features

- **Automated Data Pipeline**: Seamlessly extracts weather data from an API, processes it, and stores it in a structured format.
- **Actionable Insights**: Provides clean, reliable weather data for downstream analysis, enabling applications in forecasting, agriculture, and climate monitoring.
- **Highly Scalable**: Modular architecture to handle large datasets and integrate additional data sources.
- **Robust Orchestration**: Apache Airflow schedules, monitors, and manages all pipeline tasks efficiently.
- **Containerized Environment**: Leveraging Docker and Astronomer ensures portability and consistency across different environments.

## Architecture

The project uses a modern ETL pipeline architecture:
1. **Extract**:
   - Weather data is retrieved from a public API (e.g., OpenWeatherMap).
2. **Transform**:
   - Raw data undergoes validation, cleansing, and restructuring using Python scripts.
3. **Load**:
   - The transformed data is loaded into a PostgreSQL database for storage and querying.


---

## Tools & Technologies

- **Apache Airflow**: Task orchestration and scheduling.
- **Python**: Data extraction, transformation, and script-based processing.
- **PostgreSQL**: Relational database for efficient data storage and querying.
- **Docker**: Containerized deployment ensuring portability and ease of use.
- **Astronomer**: Airflow-as-a-Service platform for seamless pipeline management.
- **API Integration**: Utilized REST APIs for real-time weather data.

---

## Setup Instructions

Follow these steps to set up and run the project locally:

### Prerequisites

- Install [Docker](https://www.docker.com/get-started) and [Docker Compose](https://docs.docker.com/compose/).
- Clone the repository:
  ```bash
  git clone https://github.com/anshuprojects/airflow_implementation_e2e.git
  cd airflow_implementation_e2e

- Install Astronomer

## Run the Pipeline
- Start the Docker Environment:
  ```bash
  docker-compose up -d

- Access the Airflow Web Server:
  URL: http://localhost:8080
  Default credentials: admin / admin.

- Trigger the DAG:
   Log in to Airflow, navigate to the DAGs tab, and trigger the ETL pipeline DAG.

- Query the Data:
   Access PostgreSQL to verify and analyze the stored data:
   ```bash
   docker exec -it <postgres-container-name> psql -U postgres -d postgres
