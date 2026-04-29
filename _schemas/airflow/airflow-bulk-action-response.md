---
description: Serializer for individual bulk action responses. Represents the outcome of a single bulk operation (create, update, or delete). The response includes a list of successful keys and any errors encountered during the operation. This structure helps users understand which key actions succeeded and which failed.
layout: schema
name: BulkActionResponse
properties_list:
- description: A list of unique id/key representing successful operations.
  name: success
  type: array
- description: A list of errors encountered during the operation, each containing details about the issue.
  name: errors
  type: array
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-bulk-action-response-schema.json
slug: airflow-bulk-action-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-action-response-schema.json\",\n  \"title\": \"BulkActionResponse\",\n  \"description\": \"Serializer for individual bulk action responses.\\n\\nRepresents the outcome of a single bulk operation (create, update, or delete).\\nThe response includes a list of successful keys and any errors encountered during the operation.\\nThis structure helps users understand which key actions succeeded and which failed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Success\",\n      \"description\": \"A list of unique id/key representing successful operations.\",\n      \"default\": []\n    },\n    \"errors\": {\n      \"items\": {\n        \"additionalProperties\": true,\n        \"\
  type\": \"object\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Errors\",\n      \"description\": \"A list of errors encountered during the operation, each containing details about the issue.\",\n      \"default\": []\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-action-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BulkActionResponse
---
