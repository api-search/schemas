---
description: Serializer for Plugin FastAPI root middleware responses.
layout: schema
name: FastAPIRootMiddlewareResponse
properties_list:
- description: ''
  name: middleware
  type: string
- description: ''
  name: name
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-fast-api-root-middleware-response-schema.json
slug: airflow-fast-api-root-middleware-response
source_filename: airflow-fast-api-root-middleware-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-fast-api-root-middleware-response-schema.json\",\n  \"title\": \"FastAPIRootMiddlewareResponse\",\n  \"description\": \"Serializer for Plugin FastAPI root middleware responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"middleware\": {\n      \"type\": \"string\",\n      \"title\": \"Middleware\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    }\n  },\n  \"required\": [\n    \"middleware\",\n    \"name\"\n  ],\n  \"additionalProperties\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-fast-api-root-middleware-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: FastAPIRootMiddlewareResponse
---
