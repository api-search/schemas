---
description: The section of configuration.
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
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-config-section-schema.json
slug: openapi.yaml-config-section
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-config-section-schema.json\",\n  \"title\": \"ConfigSection\",\n  \"description\": \"The section of configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"options\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConfigOption\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-config-section-schema.json
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
title: ConfigSection
---
