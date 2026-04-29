---
description: HTTPException Model used for error response.
layout: schema
name: HTTPExceptionResponse
properties_list:
- description: ''
  name: detail
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-http-exception-response-schema.json
slug: airflow-http-exception-response
source_filename: airflow-http-exception-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-http-exception-response-schema.json\",\n  \"title\": \"HTTPExceptionResponse\",\n  \"description\": \"HTTPException Model used for error response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detail\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"additionalProperties\": true,\n          \"type\": \"object\"\n        }\n      ],\n      \"title\": \"Detail\"\n    }\n  },\n  \"required\": [\n    \"detail\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-http-exception-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: HTTPExceptionResponse
---
