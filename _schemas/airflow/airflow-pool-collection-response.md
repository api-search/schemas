---
description: Pool Collection serializer for responses.
layout: schema
name: PoolCollectionResponse
properties_list:
- description: ''
  name: pools
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-pool-collection-response-schema.json
slug: airflow-pool-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-pool-collection-response-schema.json\",\n  \"title\": \"PoolCollectionResponse\",\n  \"description\": \"Pool Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pools\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PoolResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Pools\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"pools\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-pool-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: PoolCollectionResponse
---
