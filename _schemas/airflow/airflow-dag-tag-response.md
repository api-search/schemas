---
description: DAG Tag serializer for responses.
layout: schema
name: DagTagResponse
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: dag_id
  type: string
- description: ''
  name: dag_display_name
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-tag-response-schema.json
slug: airflow-dag-tag-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-tag-response-schema.json\",\n  \"title\": \"DagTagResponse\",\n  \"description\": \"DAG Tag serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"dag_id\",\n    \"dag_display_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-tag-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DagTagResponse
---
