---
description: Task collection serializer for responses.
layout: schema
name: TaskCollectionResponse
properties_list:
- description: ''
  name: tasks
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-collection-response-schema.json
slug: airflow-task-collection-response
source_filename: airflow-task-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-collection-response-schema.json\",\n  \"title\": \"TaskCollectionResponse\",\n  \"description\": \"Task collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tasks\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Tasks\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"tasks\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskCollectionResponse
---
