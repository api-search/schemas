---
description: DAG Warning serializer for responses.
layout: schema
name: DAGWarningResponse
properties_list:
- description: ''
  name: dag_id
  type: string
- description: ''
  name: warning_type
  type: object
- description: ''
  name: message
  type: string
- description: ''
  name: timestamp
  type: string
- description: ''
  name: dag_display_name
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-warning-response-schema.json
slug: airflow-dag-warning-response
source_filename: airflow-dag-warning-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-warning-response-schema.json\",\n  \"title\": \"DAGWarningResponse\",\n  \"description\": \"DAG Warning serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"warning_type\": {\n      \"$ref\": \"#/components/schemas/DagWarningType\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"title\": \"Message\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Timestamp\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    }\n  },\n  \"required\": [\n    \"dag_id\",\n    \"warning_type\",\n    \"message\",\n    \"timestamp\",\n    \"dag_display_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-warning-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGWarningResponse
---
