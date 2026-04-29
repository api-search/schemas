---
description: Asset event collection response.
layout: schema
name: AssetEventCollectionResponse
properties_list:
- description: ''
  name: asset_events
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-asset-event-collection-response-schema.json
slug: airflow-asset-event-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-event-collection-response-schema.json\",\n  \"title\": \"AssetEventCollectionResponse\",\n  \"description\": \"Asset event collection response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"asset_events\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AssetEventResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Asset Events\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"asset_events\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-event-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: AssetEventCollectionResponse
---
