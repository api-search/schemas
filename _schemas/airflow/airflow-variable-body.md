---
description: Variable serializer for bodies.
layout: schema
name: VariableBody
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: value
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: team_name
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-variable-body-schema.json
slug: airflow-variable-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-variable-body-schema.json\",\n  \"title\": \"VariableBody\",\n  \"description\": \"Variable serializer for bodies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"maxLength\": 250,\n      \"title\": \"Key\"\n    },\n    \"value\": {\n      \"$ref\": \"#/components/schemas/JsonValue\"\n    },\n    \"description\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Description\"\n    },\n    \"team_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"maxLength\": 50\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Team Name\"\n    }\n  },\n  \"required\": [\n    \"key\"\
  ,\n    \"value\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-variable-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: VariableBody
---
