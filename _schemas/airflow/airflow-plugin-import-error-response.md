---
description: Plugin Import Error serializer for responses.
layout: schema
name: PluginImportErrorResponse
properties_list:
- description: ''
  name: source
  type: string
- description: ''
  name: error
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-plugin-import-error-response-schema.json
slug: airflow-plugin-import-error-response
source_filename: airflow-plugin-import-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-plugin-import-error-response-schema.json\",\n  \"title\": \"PluginImportErrorResponse\",\n  \"description\": \"Plugin Import Error serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"title\": \"Source\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"title\": \"Error\"\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"error\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-plugin-import-error-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: PluginImportErrorResponse
---
