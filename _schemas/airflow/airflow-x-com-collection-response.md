---
description: XCom Collection serializer for responses.
layout: schema
name: XComCollectionResponse
properties_list:
- description: ''
  name: xcom_entries
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-x-com-collection-response-schema.json
slug: airflow-x-com-collection-response
source_filename: airflow-x-com-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-x-com-collection-response-schema.json\",\n  \"title\": \"XComCollectionResponse\",\n  \"description\": \"XCom Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"xcom_entries\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/XComResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Xcom Entries\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"xcom_entries\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-x-com-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: XComCollectionResponse
---
