---
description: Job schema from Apache Airflow API
layout: schema
name: Job
properties_list:
- description: ''
  name: dag_id
  type: string
- description: ''
  name: end_date
  type: string
- description: ''
  name: executor_class
  type: string
- description: ''
  name: hostname
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: job_type
  type: string
- description: ''
  name: latest_heartbeat
  type: string
- description: ''
  name: start_date
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: unixname
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-job-schema.json
slug: openapi.yaml-job
source_filename: openapi.yaml-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"Job schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"end_date\": {\n      \"format\": \"datetime\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"executor_class\": {\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"hostname\": {\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"job_type\": {\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"latest_heartbeat\": {\n      \"format\": \"datetime\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"start_date\"\
  : {\n      \"format\": \"datetime\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"unixname\": {\n      \"nullable\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-job-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: Job
---
