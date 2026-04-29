---
description: DAG Run Collection serializer for responses.
layout: schema
name: DAGRunCollectionResponse
properties_list:
- description: ''
  name: dag_runs
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-run-collection-response-schema.json
slug: airflow-dag-run-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-collection-response-schema.json\",\n  \"title\": \"DAGRunCollectionResponse\",\n  \"description\": \"DAG Run Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_runs\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DAGRunResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Dag Runs\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"dag_runs\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGRunCollectionResponse
---
