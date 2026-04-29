---
description: Create asset events request.
layout: schema
name: CreateAssetEventsBody
properties_list:
- description: ''
  name: asset_id
  type: integer
- description: ''
  name: partition_key
  type: object
- description: ''
  name: extra
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-create-asset-events-body-schema.json
slug: airflow-create-asset-events-body
source_filename: airflow-create-asset-events-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-create-asset-events-body-schema.json\",\n  \"title\": \"CreateAssetEventsBody\",\n  \"description\": \"Create asset events request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"asset_id\": {\n      \"type\": \"integer\",\n      \"title\": \"Asset Id\"\n    },\n    \"partition_key\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Partition Key\"\n    },\n    \"extra\": {\n      \"additionalProperties\": true,\n      \"type\": \"object\",\n      \"title\": \"Extra\"\n    }\n  },\n  \"required\": [\n    \"asset_id\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-create-asset-events-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: CreateAssetEventsBody
---
