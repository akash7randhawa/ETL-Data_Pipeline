# ETL-Data_Pipeline


## Overview

This repository contains the code and documentation for an ETL (Extract, Transform, Load) pipeline that extracts data from an Amazon S3 bucket, creates an EMR (Elastic MapReduce) crawler to catalog the data, and transfers the cataloged data to Snowflake for analytics storage. This README provides an overview of the project, its components, and instructions on how to set it up and use it.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Usage](#usage)
- [Contributing](#contributing)

## Prerequisites

Before you begin, ensure you have the following prerequisites:

- **Amazon Web Services (AWS) Account**: You'll need access to AWS services, including S3, EMR, and IAM.
- **Snowflake Account**: You'll need a Snowflake account and access credentials.
- **Python 3.7+**: Ensure you have Python installed on your local machine.


## Setup

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/akash7randhawa/ETL-Data_Pipeline.git
   ```

2. Install the required Python packages:

3. Configure your AWS credentials and Snowflake connection details in the `airflow_emr_s3_snowflake_setup.txt` file, respectively.

4. Update the EMR Crawler configuration in `airflow_emr_spark_s3_snowflake.py` to match your data source and catalog preferences.

## Usage

1. Run the ETL pipeline:

   ```bash
   python airflow_emr_spark_s3_snowflake.py
   ```

   This will extract data from the specified S3 bucket, create an EMR Crawler to catalog the data, and transfer the cataloged data to Snowflake.

2. Monitor the ETL process for any errors or logs in the console.

## Contributing

If you'd like to contribute to this project, please follow these guidelines:

1. Fork the repository on GitHub.
2. Create a new branch for your feature or bug fix: `git checkout -b feature-name`.
3. Make your changes and commit them with clear and concise messages.
4. Push your changes to your fork: `git push origin feature-name`.
5. Submit a pull request with a description of your changes.

---

Please feel free to reach out to the project maintainers or open issues if you encounter any problems or have suggestions for improvements. Enjoy using this ETL pipeline with EMR Crawler and Snowflake integration!
