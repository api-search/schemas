---
description: The option of configuration.
layout: schema
name: ConfigOption
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: value
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-config-option-schema.json
slug: openapi.yaml-config-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-config-option-schema.json\",\n  \"title\": \"ConfigOption\",\n  \"description\": \"The option of configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-config-option-schema.json
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
title: ConfigOption
---
