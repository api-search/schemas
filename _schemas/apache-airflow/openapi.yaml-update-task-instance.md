---
description: UpdateTaskInstance schema from Apache Airflow API
layout: schema
name: UpdateTaskInstance
properties_list:
- description: If set, don't actually run this operation. The response will contain the task instance planned to be affected, but won't be modified in any way.
  name: dry_run
  type: boolean
- description: Expected new state.
  name: new_state
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-update-task-instance-schema.json
slug: openapi.yaml-update-task-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-update-task-instance-schema.json\",\n  \"title\": \"UpdateTaskInstance\",\n  \"description\": \"UpdateTaskInstance schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dry_run\": {\n      \"default\": false,\n      \"description\": \"If set, don't actually run this operation. The response will contain the task instance\\nplanned to be affected, but won't be modified in any way.\\n\",\n      \"type\": \"boolean\"\n    },\n    \"new_state\": {\n      \"description\": \"Expected new state.\",\n      \"enum\": [\n        \"success\",\n        \"failed\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-update-task-instance-schema.json
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
title: UpdateTaskInstance
---
