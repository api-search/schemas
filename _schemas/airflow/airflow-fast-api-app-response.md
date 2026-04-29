---
description: Serializer for Plugin FastAPI App responses.
layout: schema
name: FastAPIAppResponse
properties_list:
- description: ''
  name: app
  type: string
- description: ''
  name: url_prefix
  type: string
- description: ''
  name: name
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-fast-api-app-response-schema.json
slug: airflow-fast-api-app-response
source_filename: airflow-fast-api-app-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-fast-api-app-response-schema.json\",\n  \"title\": \"FastAPIAppResponse\",\n  \"description\": \"Serializer for Plugin FastAPI App responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app\": {\n      \"type\": \"string\",\n      \"title\": \"App\"\n    },\n    \"url_prefix\": {\n      \"type\": \"string\",\n      \"title\": \"Url Prefix\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    }\n  },\n  \"required\": [\n    \"app\",\n    \"url_prefix\",\n    \"name\"\n  ],\n  \"additionalProperties\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-fast-api-app-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: FastAPIAppResponse
---
