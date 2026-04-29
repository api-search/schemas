---
description: ''
layout: schema
name: Run
properties_list:
- description: ''
  name: job_id
  type: integer
- description: The canonical identifier of the run.
  name: run_id
  type: integer
- description: ''
  name: run_name
  type: string
- description: ''
  name: number_in_job
  type: integer
- description: ''
  name: original_attempt_run_id
  type: integer
- description: ''
  name: state
  type: object
- description: ''
  name: tasks
  type: array
- description: ''
  name: job_clusters
  type: array
- description: ''
  name: cluster_spec
  type: object
- description: ''
  name: cluster_instance
  type: object
- description: The start time of the run in epoch milliseconds.
  name: start_time
  type: integer
- description: Setup duration in milliseconds.
  name: setup_duration
  type: integer
- description: Execution duration in milliseconds.
  name: execution_duration
  type: integer
- description: Cleanup duration in milliseconds.
  name: cleanup_duration
  type: integer
- description: End time in epoch milliseconds.
  name: end_time
  type: integer
- description: ''
  name: trigger
  type: string
- description: ''
  name: run_type
  type: string
- description: ''
  name: attempt_number
  type: integer
- description: ''
  name: creator_user_name
  type: string
- description: URL of the run page in the Databricks workspace.
  name: run_page_url
  type: string
- description: ''
  name: format
  type: string
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-run-schema.json
slug: databricks-run
source_filename: databricks-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Run\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job_id\": {\n      \"type\": \"integer\"\n    },\n    \"run_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The canonical identifier of the run.\"\n    },\n    \"run_name\": {\n      \"type\": \"string\"\n    },\n    \"number_in_job\": {\n      \"type\": \"integer\"\n    },\n    \"original_attempt_run_id\": {\n      \"type\": \"integer\"\n    },\n    \"state\": {\n      \"type\": \"object\"\n    },\n    \"tasks\": {\n      \"type\": \"array\"\n    },\n    \"job_clusters\": {\n      \"type\": \"array\"\n    },\n    \"cluster_spec\": {\n      \"type\": \"object\"\n    },\n    \"cluster_instance\": {\n      \"type\": \"object\"\n    },\n    \"start_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The start time of the run in epoch milliseconds.\"\n    },\n    \"setup_duration\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Setup duration in milliseconds.\"\n    },\n    \"execution_duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Execution duration in milliseconds.\"\n    },\n    \"cleanup_duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Cleanup duration in milliseconds.\"\n    },\n    \"end_time\": {\n      \"type\": \"integer\",\n      \"description\": \"End time in epoch milliseconds.\"\n    },\n    \"trigger\": {\n      \"type\": \"string\"\n    },\n    \"run_type\": {\n      \"type\": \"string\"\n    },\n    \"attempt_number\": {\n      \"type\": \"integer\"\n    },\n    \"creator_user_name\": {\n      \"type\": \"string\"\n    },\n    \"run_page_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the run page in the Databricks workspace.\"\n    },\n    \"format\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-run-schema.json
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
title: Run
---
