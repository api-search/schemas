---
description: DAG Tags Collection serializer for responses.
layout: schema
name: DAGTagCollectionResponse
properties_list:
- description: ''
  name: tags
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-tag-collection-response-schema.json
slug: airflow-dag-tag-collection-response
source_filename: airflow-dag-tag-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-tag-collection-response-schema.json\",\n  \"title\": \"DAGTagCollectionResponse\",\n  \"description\": \"DAG Tags Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Tags\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"tags\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-tag-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGTagCollectionResponse
---
