---
description: Trigger schema from Apache Airflow API
layout: schema
name: Trigger
properties_list:
- description: ''
  name: classpath
  type: string
- description: ''
  name: created_date
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: kwargs
  type: string
- description: ''
  name: triggerer_id
  type: integer
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-trigger-schema.json
slug: openapi.yaml-trigger
source_filename: openapi.yaml-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-trigger-schema.json\",\n  \"title\": \"Trigger\",\n  \"description\": \"Trigger schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"classpath\": {\n      \"type\": \"string\"\n    },\n    \"created_date\": {\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"kwargs\": {\n      \"type\": \"string\"\n    },\n    \"triggerer_id\": {\n      \"nullable\": true,\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-trigger-schema.json
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
title: Trigger
---
