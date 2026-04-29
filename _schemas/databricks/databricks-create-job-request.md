---
description: ''
layout: schema
name: CreateJobRequest
properties_list:
- description: The name of the job.
  name: name
  type: string
- description: A list of task specifications to be executed by this job. For single-task jobs, use the top-level task fields instead.
  name: tasks
  type: array
- description: A list of job cluster specifications that can be shared and reused by tasks in this job.
  name: job_clusters
  type: array
- description: ''
  name: notification_settings
  type: object
- description: Maximum allowed duration for the job. If exceeded, the job is set to a TIMED_OUT life cycle state. 0 means no timeout.
  name: timeout_seconds
  type: integer
- description: Continuous job settings for streaming workloads.
  name: continuous
  type: object
- description: Trigger settings for file arrival-based jobs.
  name: trigger
  type: object
- description: Maximum number of concurrent runs for the job. Setting to 1 ensures only one run at a time.
  name: max_concurrent_runs
  type: integer
- description: Tags for the job.
  name: tags
  type: object
- description: The format of the job.
  name: format
  type: string
- description: Queue settings for the job.
  name: queue
  type: object
- description: Job-level parameter definitions.
  name: parameters
  type: array
- description: Identity to run the job as.
  name: run_as
  type: object
- description: ''
  name: access_control_list
  type: array
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-create-job-request-schema.json
slug: databricks-create-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateJobRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job.\"\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"description\": \"A list of task specifications to be executed by this job. For single-task jobs, use the top-level task fields instead.\"\n    },\n    \"job_clusters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of job cluster specifications that can be shared and reused by tasks in this job.\"\n    },\n    \"notification_settings\": {\n      \"type\": \"object\"\n    },\n    \"timeout_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum allowed duration for the job. If exceeded, the job is set to a TIMED_OUT life cycle state. 0 means no timeout.\"\n    },\n    \"continuous\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Continuous job settings for streaming workloads.\"\n    },\n    \"trigger\": {\n      \"type\": \"object\",\n      \"description\": \"Trigger settings for file arrival-based jobs.\"\n    },\n    \"max_concurrent_runs\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of concurrent runs for the job. Setting to 1 ensures only one run at a time.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags for the job.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The format of the job.\"\n    },\n    \"queue\": {\n      \"type\": \"object\",\n      \"description\": \"Queue settings for the job.\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Job-level parameter definitions.\"\n    },\n    \"run_as\": {\n      \"type\": \"object\",\n      \"description\": \"Identity to run the job as.\"\n    },\n    \"access_control_list\": {\n      \"type\": \"array\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-create-job-request-schema.json
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
title: CreateJobRequest
---
