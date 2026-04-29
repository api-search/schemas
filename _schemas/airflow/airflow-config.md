---
description: List of config sections with their options.
layout: schema
name: Config
properties_list:
- description: ''
  name: sections
  type: array
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-config-schema.json
slug: airflow-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-config-schema.json\",\n  \"title\": \"Config\",\n  \"description\": \"List of config sections with their options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sections\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConfigSection\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Sections\"\n    }\n  },\n  \"required\": [\n    \"sections\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-config-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: Config
---
