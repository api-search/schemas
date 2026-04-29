---
description: TaskInstanceReference schema from Apache Airflow API
layout: schema
name: TaskInstanceReference
properties_list:
- description: The DAG ID.
  name: dag_id
  type: string
- description: The DAG run ID.
  name: dag_run_id
  type: string
- description: ''
  name: execution_date
  type: string
- description: The task ID.
  name: task_id
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-task-instance-reference-schema.json
slug: openapi.yaml-task-instance-reference
source_filename: openapi.yaml-task-instance-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-instance-reference-schema.json\",\n  \"title\": \"TaskInstanceReference\",\n  \"description\": \"TaskInstanceReference schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"description\": \"The DAG ID.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"dag_run_id\": {\n      \"description\": \"The DAG run ID.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"execution_date\": {\n      \"format\": \"datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"task_id\": {\n      \"description\": \"The task ID.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-instance-reference-schema.json
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
title: TaskInstanceReference
---
