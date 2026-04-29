---
description: Asset collection response.
layout: schema
name: AssetCollectionResponse
properties_list:
- description: ''
  name: assets
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-asset-collection-response-schema.json
slug: airflow-asset-collection-response
source_filename: airflow-asset-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-collection-response-schema.json\",\n  \"title\": \"AssetCollectionResponse\",\n  \"description\": \"Asset collection response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assets\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AssetResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Assets\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"assets\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: AssetCollectionResponse
---
