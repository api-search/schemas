---
description: DAG Stats serializer for responses.
layout: schema
name: DagStatsResponse
properties_list:
- description: ''
  name: dag_id
  type: string
- description: ''
  name: dag_display_name
  type: string
- description: ''
  name: stats
  type: array
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-stats-response-schema.json
slug: airflow-dag-stats-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-stats-response-schema.json\",\n  \"title\": \"DagStatsResponse\",\n  \"description\": \"DAG Stats serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    },\n    \"stats\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DagStatsStateResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Stats\"\n    }\n  },\n  \"required\": [\n    \"dag_id\",\n    \"dag_display_name\",\n    \"stats\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-stats-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DagStatsResponse
---
