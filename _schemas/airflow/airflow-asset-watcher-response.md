---
description: Asset watcher serializer for responses.
layout: schema
name: AssetWatcherResponse
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: trigger_id
  type: integer
- description: ''
  name: created_date
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-asset-watcher-response-schema.json
slug: airflow-asset-watcher-response
source_filename: airflow-asset-watcher-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-watcher-response-schema.json\",\n  \"title\": \"AssetWatcherResponse\",\n  \"description\": \"Asset watcher serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"trigger_id\": {\n      \"type\": \"integer\",\n      \"title\": \"Trigger Id\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Created Date\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"trigger_id\",\n    \"created_date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-watcher-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: AssetWatcherResponse
---
