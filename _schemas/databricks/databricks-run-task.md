---
description: ''
layout: schema
name: RunTask
properties_list:
- description: ''
  name: run_id
  type: integer
- description: ''
  name: task_key
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: state
  type: object
- description: ''
  name: depends_on
  type: array
- description: ''
  name: existing_cluster_id
  type: string
- description: ''
  name: notebook_task
  type: object
- description: ''
  name: spark_jar_task
  type: object
- description: ''
  name: spark_python_task
  type: object
- description: ''
  name: sql_task
  type: object
- description: ''
  name: start_time
  type: integer
- description: ''
  name: setup_duration
  type: integer
- description: ''
  name: execution_duration
  type: integer
- description: ''
  name: cleanup_duration
  type: integer
- description: ''
  name: end_time
  type: integer
- description: ''
  name: cluster_instance
  type: object
- description: ''
  name: attempt_number
  type: integer
- description: ''
  name: libraries
  type: array
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-run-task-schema.json
slug: databricks-run-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RunTask\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"run_id\": {\n      \"type\": \"integer\"\n    },\n    \"task_key\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"object\"\n    },\n    \"depends_on\": {\n      \"type\": \"array\"\n    },\n    \"existing_cluster_id\": {\n      \"type\": \"string\"\n    },\n    \"notebook_task\": {\n      \"type\": \"object\"\n    },\n    \"spark_jar_task\": {\n      \"type\": \"object\"\n    },\n    \"spark_python_task\": {\n      \"type\": \"object\"\n    },\n    \"sql_task\": {\n      \"type\": \"object\"\n    },\n    \"start_time\": {\n      \"type\": \"integer\"\n    },\n    \"setup_duration\": {\n      \"type\": \"integer\"\n    },\n    \"execution_duration\": {\n      \"type\": \"integer\"\n    },\n    \"cleanup_duration\": {\n      \"type\": \"integer\"\
  \n    },\n    \"end_time\": {\n      \"type\": \"integer\"\n    },\n    \"cluster_instance\": {\n      \"type\": \"object\"\n    },\n    \"attempt_number\": {\n      \"type\": \"integer\"\n    },\n    \"libraries\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-run-task-schema.json
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
title: RunTask
---
