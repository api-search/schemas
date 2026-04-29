---
description: ImportError schema from Apache Airflow API
layout: schema
name: ImportError
properties_list:
- description: The filename
  name: filename
  type: string
- description: The import error ID.
  name: import_error_id
  type: integer
- description: The full stackstrace..
  name: stack_trace
  type: string
- description: The time when this error was created.
  name: timestamp
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-import-error-schema.json
slug: openapi.yaml-import-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-import-error-schema.json\",\n  \"title\": \"ImportError\",\n  \"description\": \"ImportError schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filename\": {\n      \"description\": \"The filename\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"import_error_id\": {\n      \"description\": \"The import error ID.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"stack_trace\": {\n      \"description\": \"The full stackstrace..\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"description\": \"The time when this error was created.\",\n      \"format\": \"datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-import-error-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: ImportError
---
