---
description: Variable serializer for responses.
layout: schema
name: VariableResponse
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: value
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: is_encrypted
  type: boolean
- description: ''
  name: team_name
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-variable-response-schema.json
slug: airflow-variable-response
source_filename: airflow-variable-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-variable-response-schema.json\",\n  \"title\": \"VariableResponse\",\n  \"description\": \"Variable serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"title\": \"Key\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"title\": \"Value\"\n    },\n    \"description\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Description\"\n    },\n    \"is_encrypted\": {\n      \"type\": \"boolean\",\n      \"title\": \"Is Encrypted\"\n    },\n    \"team_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\"\
  : \"Team Name\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"value\",\n    \"description\",\n    \"is_encrypted\",\n    \"team_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-variable-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: VariableResponse
---
