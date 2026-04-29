---
description: Serializer for a xcom item.
layout: schema
name: XComResponse
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: timestamp
  type: string
- description: ''
  name: logical_date
  type: object
- description: ''
  name: map_index
  type: integer
- description: ''
  name: task_id
  type: string
- description: ''
  name: dag_id
  type: string
- description: ''
  name: run_id
  type: string
- description: ''
  name: dag_display_name
  type: string
- description: ''
  name: task_display_name
  type: string
- description: ''
  name: run_after
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-x-com-response-schema.json
slug: airflow-x-com-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-x-com-response-schema.json\",\n  \"title\": \"XComResponse\",\n  \"description\": \"Serializer for a xcom item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"title\": \"Key\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Timestamp\"\n    },\n    \"logical_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Logical Date\"\n    },\n    \"map_index\": {\n      \"type\": \"integer\",\n      \"title\": \"Map Index\"\n    },\n    \"task_id\": {\n      \"type\": \"string\",\n      \"title\": \"Task Id\"\n    },\n    \"dag_id\": {\n     \
  \ \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"run_id\": {\n      \"type\": \"string\",\n      \"title\": \"Run Id\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    },\n    \"task_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Task Display Name\"\n    },\n    \"run_after\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Run After\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"timestamp\",\n    \"logical_date\",\n    \"map_index\",\n    \"task_id\",\n    \"dag_id\",\n    \"run_id\",\n    \"dag_display_name\",\n    \"task_display_name\",\n    \"run_after\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-x-com-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: XComResponse
---
