---
description: ''
layout: schema
name: Job
properties_list:
- description: The canonical identifier for this job.
  name: job_id
  type: integer
- description: The email of the user who created the job.
  name: creator_user_name
  type: string
- description: The email of the user the job runs as.
  name: run_as_user_name
  type: string
- description: The time the job was created in epoch milliseconds.
  name: created_time
  type: integer
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-job-schema.json
slug: databricks-job
source_filename: databricks-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The canonical identifier for this job.\"\n    },\n    \"creator_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"The email of the user who created the job.\"\n    },\n    \"run_as_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"The email of the user the job runs as.\"\n    },\n    \"created_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time the job was created in epoch milliseconds.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-job-schema.json
tags:
- AI
- Analytics
- Apache Spark
- Big Data
- Clean Rooms
- Cloud Computing
- Data
- Data Analytics
- Data Engineering
- Data Governance
- Delta Lake
- Delta Sharing
- ETL
- Identity Management
- Lakehouse
- Machine Learning
- MLflow
- Model Serving
- Security
- SQL
- Unity Catalog
- Vector Search
- Visualize
title: Job
---
