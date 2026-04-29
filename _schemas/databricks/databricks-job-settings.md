---
description: ''
layout: schema
name: JobSettings
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: tasks
  type: array
- description: ''
  name: job_clusters
  type: array
- description: ''
  name: timeout_seconds
  type: integer
- description: ''
  name: max_concurrent_runs
  type: integer
- description: ''
  name: tags
  type: object
- description: ''
  name: format
  type: string
- description: ''
  name: queue
  type: object
- description: ''
  name: continuous
  type: object
- description: ''
  name: parameters
  type: array
- description: ''
  name: run_as
  type: object
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-job-settings-schema.json
slug: databricks-job-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"tasks\": {\n      \"type\": \"array\"\n    },\n    \"job_clusters\": {\n      \"type\": \"array\"\n    },\n    \"timeout_seconds\": {\n      \"type\": \"integer\"\n    },\n    \"max_concurrent_runs\": {\n      \"type\": \"integer\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    },\n    \"format\": {\n      \"type\": \"string\"\n    },\n    \"queue\": {\n      \"type\": \"object\"\n    },\n    \"continuous\": {\n      \"type\": \"object\"\n    },\n    \"parameters\": {\n      \"type\": \"array\"\n    },\n    \"run_as\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-job-settings-schema.json
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
title: JobSettings
---
