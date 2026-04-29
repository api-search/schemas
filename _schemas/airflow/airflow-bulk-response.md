---
description: Serializer for responses to bulk entity operations. This represents the results of create, update, and delete actions performed on entity in bulk. Each action (if requested) is represented as a field containing details about successful keys and any encountered errors. Fields are populated in the response only if the respective action was part of the request, else are set None.
layout: schema
name: BulkResponse
properties_list:
- description: Details of the bulk create operation, including successful keys and errors.
  name: create
  type: object
- description: Details of the bulk update operation, including successful keys and errors.
  name: update
  type: object
- description: Details of the bulk delete operation, including successful keys and errors.
  name: delete
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-bulk-response-schema.json
slug: airflow-bulk-response
source_filename: airflow-bulk-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-response-schema.json\",\n  \"title\": \"BulkResponse\",\n  \"description\": \"Serializer for responses to bulk entity operations.\\n\\nThis represents the results of create, update, and delete actions performed on entity in bulk.\\nEach action (if requested) is represented as a field containing details about successful keys and any encountered errors.\\nFields are populated in the response only if the respective action was part of the request, else are set None.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"create\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BulkActionResponse\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"description\": \"Details of the bulk create operation, including successful keys and errors.\"\
  \n    },\n    \"update\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BulkActionResponse\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"description\": \"Details of the bulk update operation, including successful keys and errors.\"\n    },\n    \"delete\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BulkActionResponse\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"description\": \"Details of the bulk delete operation, including successful keys and errors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BulkResponse
---
