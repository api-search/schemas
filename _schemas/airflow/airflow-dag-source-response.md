---
description: DAG Source serializer for responses.
layout: schema
name: DAGSourceResponse
properties_list:
- description: ''
  name: content
  type: object
- description: ''
  name: dag_id
  type: string
- description: ''
  name: version_number
  type: object
- description: ''
  name: dag_display_name
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-source-response-schema.json
slug: airflow-dag-source-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-source-response-schema.json\",\n  \"title\": \"DAGSourceResponse\",\n  \"description\": \"DAG Source serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Content\"\n    },\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"version_number\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Version Number\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    }\n  },\n  \"required\": [\n    \"content\"\
  ,\n    \"dag_id\",\n    \"version_number\",\n    \"dag_display_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-source-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGSourceResponse
---
