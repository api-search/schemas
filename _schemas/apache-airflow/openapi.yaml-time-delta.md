---
description: Time delta
layout: schema
name: TimeDelta
properties_list:
- description: ''
  name: __type
  type: string
- description: ''
  name: days
  type: integer
- description: ''
  name: microseconds
  type: integer
- description: ''
  name: seconds
  type: integer
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-time-delta-schema.json
slug: openapi.yaml-time-delta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-time-delta-schema.json\",\n  \"title\": \"TimeDelta\",\n  \"description\": \"Time delta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"__type\": {\n      \"type\": \"string\"\n    },\n    \"days\": {\n      \"type\": \"integer\"\n    },\n    \"microseconds\": {\n      \"type\": \"integer\"\n    },\n    \"seconds\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"__type\",\n    \"days\",\n    \"seconds\",\n    \"microseconds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-time-delta-schema.json
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
title: TimeDelta
---
