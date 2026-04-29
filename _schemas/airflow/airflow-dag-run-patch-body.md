---
description: DAG Run Serializer for PATCH requests.
layout: schema
name: DAGRunPatchBody
properties_list:
- description: ''
  name: state
  type: object
- description: ''
  name: note
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-run-patch-body-schema.json
slug: airflow-dag-run-patch-body
source_filename: airflow-dag-run-patch-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-patch-body-schema.json\",\n  \"title\": \"DAGRunPatchBody\",\n  \"description\": \"DAG Run Serializer for PATCH requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DAGRunPatchStates\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    },\n    \"note\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"maxLength\": 1000\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Note\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-patch-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGRunPatchBody
---
