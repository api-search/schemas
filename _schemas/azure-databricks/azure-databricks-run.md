---
description: ''
layout: schema
name: Run
properties_list:
- description: Canonical identifier of the run
  name: run_id
  type: integer
- description: ID of the job this run belongs to
  name: job_id
  type: integer
- description: Name of the run
  name: run_name
  type: string
- description: Username of the user who triggered the run
  name: creator_user_name
  type: string
- description: Sequence number of this run among all runs of the job
  name: number_in_job
  type: integer
- description: ''
  name: tasks
  type: array
- description: ''
  name: cluster_spec
  type: object
- description: ''
  name: cluster_instance
  type: object
- description: Start time of the run (epoch milliseconds)
  name: start_time
  type: integer
- description: Time spent setting up the cluster in milliseconds
  name: setup_duration
  type: integer
- description: Time spent executing the run in milliseconds
  name: execution_duration
  type: integer
- description: Time spent cleaning up after the run in milliseconds
  name: cleanup_duration
  type: integer
- description: End time of the run (epoch milliseconds)
  name: end_time
  type: integer
- description: What triggered this run
  name: trigger
  type: string
- description: ''
  name: run_type
  type: string
- description: Current attempt number of the run
  name: attempt_number
  type: integer
- description: URL of the run page in the Databricks UI
  name: run_page_url
  type: string
- description: ''
  name: format
  type: string
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-run-schema.json
slug: azure-databricks-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Run\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"run_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Canonical identifier of the run\"\n    },\n    \"job_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the job this run belongs to\"\n    },\n    \"run_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the run\"\n    },\n    \"creator_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who triggered the run\"\n    },\n    \"number_in_job\": {\n      \"type\": \"integer\",\n      \"description\": \"Sequence number of this run among all runs of the job\"\n    },\n    \"tasks\": {\n      \"type\": \"array\"\n    },\n    \"cluster_spec\": {\n      \"type\": \"object\"\n    },\n    \"cluster_instance\": {\n      \"type\": \"object\"\n    },\n    \"start_time\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Start time of the run (epoch milliseconds)\"\n    },\n    \"setup_duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Time spent setting up the cluster in milliseconds\"\n    },\n    \"execution_duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Time spent executing the run in milliseconds\"\n    },\n    \"cleanup_duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Time spent cleaning up after the run in milliseconds\"\n    },\n    \"end_time\": {\n      \"type\": \"integer\",\n      \"description\": \"End time of the run (epoch milliseconds)\"\n    },\n    \"trigger\": {\n      \"type\": \"string\",\n      \"description\": \"What triggered this run\"\n    },\n    \"run_type\": {\n      \"type\": \"string\"\n    },\n    \"attempt_number\": {\n      \"type\": \"integer\",\n      \"description\": \"Current attempt number of the run\"\n    },\n    \"run_page_url\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"URL of the run page in the Databricks UI\"\n    },\n    \"format\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-run-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: Run
---
