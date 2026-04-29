---
description: Log serializer for responses.
layout: schema
name: TaskInstancesLogResponse
properties_list:
- description: ''
  name: content
  type: object
- description: ''
  name: continuation_token
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-instances-log-response-schema.json
slug: airflow-task-instances-log-response
source_filename: airflow-task-instances-log-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instances-log-response-schema.json\",\n  \"title\": \"TaskInstancesLogResponse\",\n  \"description\": \"Log serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"anyOf\": [\n        {\n          \"items\": {\n            \"$ref\": \"#/components/schemas/StructuredLogMessage\"\n          },\n          \"type\": \"array\"\n        },\n        {\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"type\": \"array\"\n        }\n      ],\n      \"title\": \"Content\"\n    },\n    \"continuation_token\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Continuation Token\"\n    }\n  },\n  \"required\": [\n    \"content\"\
  ,\n    \"continuation_token\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instances-log-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskInstancesLogResponse
---
