---
description: Import Error Response.
layout: schema
name: ImportErrorResponse
properties_list:
- description: ''
  name: import_error_id
  type: integer
- description: ''
  name: timestamp
  type: string
- description: ''
  name: filename
  type: string
- description: ''
  name: bundle_name
  type: object
- description: ''
  name: stack_trace
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-import-error-response-schema.json
slug: airflow-import-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-import-error-response-schema.json\",\n  \"title\": \"ImportErrorResponse\",\n  \"description\": \"Import Error Response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"import_error_id\": {\n      \"type\": \"integer\",\n      \"title\": \"Import Error Id\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Timestamp\"\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"title\": \"Filename\"\n    },\n    \"bundle_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Bundle Name\"\n    },\n    \"stack_trace\": {\n      \"type\": \"string\",\n      \"title\": \"Stack Trace\"\n    }\n  },\n  \"required\": [\n \
  \   \"import_error_id\",\n    \"timestamp\",\n    \"filename\",\n    \"bundle_name\",\n    \"stack_trace\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-import-error-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ImportErrorResponse
---
