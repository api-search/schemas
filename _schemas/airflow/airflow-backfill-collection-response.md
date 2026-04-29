---
description: Backfill Collection serializer for responses.
layout: schema
name: BackfillCollectionResponse
properties_list:
- description: ''
  name: backfills
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-backfill-collection-response-schema.json
slug: airflow-backfill-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-backfill-collection-response-schema.json\",\n  \"title\": \"BackfillCollectionResponse\",\n  \"description\": \"Backfill Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"backfills\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BackfillResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Backfills\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"backfills\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-backfill-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BackfillCollectionResponse
---
