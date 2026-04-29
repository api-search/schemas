---
description: Additional links containing additional information about the task.
layout: schema
name: ExtraLink
properties_list:
- description: ''
  name: class_ref
  type: object
- description: ''
  name: href
  type: string
- description: ''
  name: name
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-extra-link-schema.json
slug: openapi.yaml-extra-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-extra-link-schema.json\",\n  \"title\": \"ExtraLink\",\n  \"description\": \"Additional links containing additional information about the task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"class_ref\": {\n      \"$ref\": \"#/components/schemas/ClassReference\"\n    },\n    \"href\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-extra-link-schema.json
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
title: ExtraLink
---
