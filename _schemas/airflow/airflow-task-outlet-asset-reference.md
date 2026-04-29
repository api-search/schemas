---
description: Task outlet reference serializer for assets.
layout: schema
name: TaskOutletAssetReference
properties_list:
- description: ''
  name: dag_id
  type: string
- description: ''
  name: task_id
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-outlet-asset-reference-schema.json
slug: airflow-task-outlet-asset-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-outlet-asset-reference-schema.json\",\n  \"title\": \"TaskOutletAssetReference\",\n  \"description\": \"Task outlet reference serializer for assets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"task_id\": {\n      \"type\": \"string\",\n      \"title\": \"Task Id\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Created At\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Updated At\"\n    }\n  },\n  \"required\": [\n    \"dag_id\",\n    \"task_id\",\n    \"created_at\",\n    \"updated_at\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-outlet-asset-reference-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskOutletAssetReference
---
