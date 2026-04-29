---
description: Asset alias serializer for responses.
layout: schema
name: AssetAliasResponse
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: group
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-asset-alias-response-schema.json
slug: airflow-asset-alias-response
source_filename: airflow-asset-alias-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-alias-response-schema.json\",\n  \"title\": \"AssetAliasResponse\",\n  \"description\": \"Asset alias serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"title\": \"Id\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"group\": {\n      \"type\": \"string\",\n      \"title\": \"Group\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"group\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-alias-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: AssetAliasResponse
---
