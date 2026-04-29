---
description: The configuration.
layout: schema
name: Config
properties_list:
- description: ''
  name: sections
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-config-schema.json
slug: openapi.yaml-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-config-schema.json\",\n  \"title\": \"Config\",\n  \"description\": \"The configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sections\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConfigSection\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-config-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: Config
---
