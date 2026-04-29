---
description: ''
layout: schema
name: TaskSettings
properties_list:
- description: Unique key for the task within the job. Must be unique among all tasks in the same job.
  name: task_key
  type: string
- description: Optional description for the task
  name: description
  type: string
- description: Tasks this task depends on. The task will not start until all dependent tasks complete successfully.
  name: depends_on
  type: array
- description: ID of an existing cluster to use for this task
  name: existing_cluster_id
  type: string
- description: Key of a job cluster specification to use. Refers to a cluster defined in the job's job_clusters field.
  name: job_cluster_key
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
  name: spark_submit_task
  type: object
- description: ''
  name: pipeline_task
  type: object
- description: ''
  name: python_wheel_task
  type: object
- description: ''
  name: sql_task
  type: object
- description: ''
  name: dbt_task
  type: object
- description: Condition for running this task based on dependencies
  name: run_if
  type: string
- description: Timeout in seconds for this individual task
  name: timeout_seconds
  type: integer
- description: Maximum number of retries for this task
  name: max_retries
  type: integer
- description: Minimum interval between retries in milliseconds
  name: min_retry_interval_millis
  type: integer
- description: Whether to retry the task if it times out
  name: retry_on_timeout
  type: boolean
- description: Libraries to install on the task cluster
  name: libraries
  type: array
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-task-settings-schema.json
slug: azure-databricks-task-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"task_key\": {\n      \"type\": \"string\",\n      \"description\": \"Unique key for the task within the job. Must be unique among all tasks in the same job.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description for the task\"\n    },\n    \"depends_on\": {\n      \"type\": \"array\",\n      \"description\": \"Tasks this task depends on. The task will not start until all dependent tasks complete successfully.\"\n    },\n    \"existing_cluster_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of an existing cluster to use for this task\"\n    },\n    \"job_cluster_key\": {\n      \"type\": \"string\",\n      \"description\": \"Key of a job cluster specification to use. Refers to a cluster defined in the job's job_clusters field.\"\n    },\n    \"notebook_task\"\
  : {\n      \"type\": \"object\"\n    },\n    \"spark_jar_task\": {\n      \"type\": \"object\"\n    },\n    \"spark_python_task\": {\n      \"type\": \"object\"\n    },\n    \"spark_submit_task\": {\n      \"type\": \"object\"\n    },\n    \"pipeline_task\": {\n      \"type\": \"object\"\n    },\n    \"python_wheel_task\": {\n      \"type\": \"object\"\n    },\n    \"sql_task\": {\n      \"type\": \"object\"\n    },\n    \"dbt_task\": {\n      \"type\": \"object\"\n    },\n    \"run_if\": {\n      \"type\": \"string\",\n      \"description\": \"Condition for running this task based on dependencies\"\n    },\n    \"timeout_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds for this individual task\"\n    },\n    \"max_retries\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of retries for this task\"\n    },\n    \"min_retry_interval_millis\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum interval between\
  \ retries in milliseconds\"\n    },\n    \"retry_on_timeout\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to retry the task if it times out\"\n    },\n    \"libraries\": {\n      \"type\": \"array\",\n      \"description\": \"Libraries to install on the task cluster\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-task-settings-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: TaskSettings
---
