---
description: An individual log message.
layout: schema
name: StructuredLogMessage
properties_list:
- description: ''
  name: timestamp
  type: string
- description: ''
  name: event
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-structured-log-message-schema.json
slug: airflow-structured-log-message
source_filename: airflow-structured-log-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-structured-log-message-schema.json\",\n  \"title\": \"StructuredLogMessage\",\n  \"description\": \"An individual log message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Timestamp\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"title\": \"Event\"\n    }\n  },\n  \"required\": [\n    \"event\"\n  ],\n  \"additionalProperties\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-structured-log-message-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: StructuredLogMessage
---
