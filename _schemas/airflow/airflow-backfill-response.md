---
description: Base serializer for Backfill.
layout: schema
name: BackfillResponse
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: dag_id
  type: string
- description: ''
  name: from_date
  type: string
- description: ''
  name: to_date
  type: string
- description: ''
  name: dag_run_conf
  type: object
- description: ''
  name: is_paused
  type: boolean
- description: ''
  name: reprocess_behavior
  type: object
- description: ''
  name: max_active_runs
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: completed_at
  type: object
- description: ''
  name: updated_at
  type: string
- description: ''
  name: dag_display_name
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-backfill-response-schema.json
slug: airflow-backfill-response
source_filename: airflow-backfill-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-backfill-response-schema.json\",\n  \"title\": \"BackfillResponse\",\n  \"description\": \"Base serializer for Backfill.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"minimum\": 0.0,\n      \"title\": \"Id\"\n    },\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"from_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"From Date\"\n    },\n    \"to_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"To Date\"\n    },\n    \"dag_run_conf\": {\n      \"anyOf\": [\n        {\n          \"additionalProperties\": true,\n          \"type\": \"object\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n  \
  \    \"title\": \"Dag Run Conf\"\n    },\n    \"is_paused\": {\n      \"type\": \"boolean\",\n      \"title\": \"Is Paused\"\n    },\n    \"reprocess_behavior\": {\n      \"$ref\": \"#/components/schemas/ReprocessBehavior\"\n    },\n    \"max_active_runs\": {\n      \"type\": \"integer\",\n      \"title\": \"Max Active Runs\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Created At\"\n    },\n    \"completed_at\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Completed At\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Updated At\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"dag_id\",\n    \"\
  from_date\",\n    \"to_date\",\n    \"dag_run_conf\",\n    \"is_paused\",\n    \"reprocess_behavior\",\n    \"max_active_runs\",\n    \"created_at\",\n    \"completed_at\",\n    \"updated_at\",\n    \"dag_display_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-backfill-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BackfillResponse
---
