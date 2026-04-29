---
description: Plugin Collection serializer.
layout: schema
name: PluginCollectionResponse
properties_list:
- description: ''
  name: plugins
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-plugin-collection-response-schema.json
slug: airflow-plugin-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-plugin-collection-response-schema.json\",\n  \"title\": \"PluginCollectionResponse\",\n  \"description\": \"Plugin Collection serializer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"plugins\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PluginResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Plugins\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"plugins\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-plugin-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: PluginCollectionResponse
---
