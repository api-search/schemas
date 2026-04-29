---
description: Config option.
layout: schema
name: ConfigOption
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: value
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-config-option-schema.json
slug: airflow-config-option
source_filename: airflow-config-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-config-option-schema.json\",\n  \"title\": \"ConfigOption\",\n  \"description\": \"Config option.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"title\": \"Key\"\n    },\n    \"value\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"prefixItems\": [\n            {\n              \"type\": \"string\"\n            },\n            {\n              \"type\": \"string\"\n            }\n          ],\n          \"type\": \"array\",\n          \"maxItems\": 2,\n          \"minItems\": 2\n        }\n      ],\n      \"title\": \"Value\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"value\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-config-option-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ConfigOption
---
