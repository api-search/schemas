---
description: Queued Event serializer for responses..
layout: schema
name: QueuedEventResponse
properties_list:
- description: ''
  name: dag_id
  type: string
- description: ''
  name: asset_id
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: dag_display_name
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-queued-event-response-schema.json
slug: airflow-queued-event-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-queued-event-response-schema.json\",\n  \"title\": \"QueuedEventResponse\",\n  \"description\": \"Queued Event serializer for responses..\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"asset_id\": {\n      \"type\": \"integer\",\n      \"title\": \"Asset Id\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Created At\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    }\n  },\n  \"required\": [\n    \"dag_id\",\n    \"asset_id\",\n    \"created_at\",\n    \"dag_display_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-queued-event-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: QueuedEventResponse
---
