---
description: Connection Collection serializer for responses.
layout: schema
name: ConnectionCollectionResponse
properties_list:
- description: ''
  name: connections
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-connection-collection-response-schema.json
slug: airflow-connection-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-connection-collection-response-schema.json\",\n  \"title\": \"ConnectionCollectionResponse\",\n  \"description\": \"Connection Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connections\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConnectionResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Connections\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"connections\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-connection-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ConnectionCollectionResponse
---
