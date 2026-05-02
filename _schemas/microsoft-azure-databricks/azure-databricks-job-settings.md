---
description: ''
layout: schema
name: JobSettings
properties_list:
- description: Optional name for the job. Default is Untitled.
  name: name
  type: string
- description: Map of tags associated with the job
  name: tags
  type: object
- description: List of task specifications for the job. A job must contain at least one task.
  name: tasks
  type: array
- description: A list of job cluster specifications that can be shared and reused by tasks.
  name: job_clusters
  type: array
- description: ''
  name: notification_settings
  type: object
- description: Timeout in seconds applied to each run of this job. Default is no timeout.
  name: timeout_seconds
  type: integer
- description: Maximum allowed number of concurrent runs of the job. Default is 1.
  name: max_concurrent_runs
  type: integer
- description: Trigger settings for file arrival events
  name: trigger
  type: object
- description: Settings for continuous job execution
  name: continuous
  type: object
- description: Format of the job. MULTI_TASK is the preferred format for creating jobs with multiple tasks.
  name: format
  type: string
- description: ''
  name: queue
  type: object
- description: Job-level parameters
  name: parameters
  type: array
- description: User or service principal to run the job as
  name: run_as
  type: object
provider_name: Azure Databricks
provider_slug: microsoft-azure-databricks
schema_file: json-schema/azure-databricks-job-settings-schema.json
slug: azure-databricks-job-settings
source_filename: azure-databricks-job-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Optional name for the job. Default is Untitled.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Map of tags associated with the job\"\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"description\": \"List of task specifications for the job. A job must contain at least one task.\"\n    },\n    \"job_clusters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of job cluster specifications that can be shared and reused by tasks.\"\n    },\n    \"notification_settings\": {\n      \"type\": \"object\"\n    },\n    \"timeout_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds applied to each run of this job. Default is no timeout.\"\n    },\n    \"max_concurrent_runs\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Maximum allowed number of concurrent runs of the job. Default is 1.\"\n    },\n    \"trigger\": {\n      \"type\": \"object\",\n      \"description\": \"Trigger settings for file arrival events\"\n    },\n    \"continuous\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for continuous job execution\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Format of the job. MULTI_TASK is the preferred format for creating jobs with multiple tasks.\"\n    },\n    \"queue\": {\n      \"type\": \"object\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Job-level parameters\"\n    },\n    \"run_as\": {\n      \"type\": \"object\",\n      \"description\": \"User or service principal to run the job as\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-databricks/refs/heads/main/json-schema/azure-databricks-job-settings-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: JobSettings
---
