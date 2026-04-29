---
description: Import Error Collection Response.
layout: schema
name: ImportErrorCollectionResponse
properties_list:
- description: ''
  name: import_errors
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-import-error-collection-response-schema.json
slug: airflow-import-error-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-import-error-collection-response-schema.json\",\n  \"title\": \"ImportErrorCollectionResponse\",\n  \"description\": \"Import Error Collection Response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"import_errors\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ImportErrorResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Import Errors\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"import_errors\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-import-error-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ImportErrorCollectionResponse
---
