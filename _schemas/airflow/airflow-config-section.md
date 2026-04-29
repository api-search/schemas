---
description: Config Section Schema.
layout: schema
name: ConfigSection
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: options
  type: array
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-config-section-schema.json
slug: airflow-config-section
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-config-section-schema.json\",\n  \"title\": \"ConfigSection\",\n  \"description\": \"Config Section Schema.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"options\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConfigOption\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Options\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"options\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-config-section-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ConfigSection
---
