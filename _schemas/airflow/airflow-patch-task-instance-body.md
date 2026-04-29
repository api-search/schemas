---
description: Request body for Clear Task Instances endpoint.
layout: schema
name: PatchTaskInstanceBody
properties_list:
- description: ''
  name: new_state
  type: object
- description: ''
  name: note
  type: object
- description: ''
  name: include_upstream
  type: boolean
- description: ''
  name: include_downstream
  type: boolean
- description: ''
  name: include_future
  type: boolean
- description: ''
  name: include_past
  type: boolean
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-patch-task-instance-body-schema.json
slug: airflow-patch-task-instance-body
source_filename: airflow-patch-task-instance-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-patch-task-instance-body-schema.json\",\n  \"title\": \"PatchTaskInstanceBody\",\n  \"description\": \"Request body for Clear Task Instances endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"new_state\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskInstanceState\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    },\n    \"note\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"maxLength\": 1000\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Note\"\n    },\n    \"include_upstream\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Upstream\",\n      \"default\": false\n    },\n    \"include_downstream\": {\n      \"type\": \"boolean\",\n\
  \      \"title\": \"Include Downstream\",\n      \"default\": false\n    },\n    \"include_future\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Future\",\n      \"default\": false\n    },\n    \"include_past\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Past\",\n      \"default\": false\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-patch-task-instance-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: PatchTaskInstanceBody
---
