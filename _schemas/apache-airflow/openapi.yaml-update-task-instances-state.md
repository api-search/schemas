---
description: UpdateTaskInstancesState schema from Apache Airflow API
layout: schema
name: UpdateTaskInstancesState
properties_list:
- description: The task instance's DAG run ID. Either set this or execution_date but not both. *New in version 2.3.0*
  name: dag_run_id
  type: string
- description: If set, don't actually run this operation. The response will contain a list of task instances planned to be affected, but won't be modified in any way.
  name: dry_run
  type: boolean
- description: The execution date. Either set this or dag_run_id but not both.
  name: execution_date
  type: string
- description: If set to true, downstream tasks are also affected.
  name: include_downstream
  type: boolean
- description: If set to True, also tasks from future DAG Runs are affected.
  name: include_future
  type: boolean
- description: If set to True, also tasks from past DAG Runs are affected.
  name: include_past
  type: boolean
- description: If set to true, upstream tasks are also affected.
  name: include_upstream
  type: boolean
- description: Expected new state.
  name: new_state
  type: string
- description: The task ID.
  name: task_id
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-update-task-instances-state-schema.json
slug: openapi.yaml-update-task-instances-state
source_filename: openapi.yaml-update-task-instances-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-update-task-instances-state-schema.json\",\n  \"title\": \"UpdateTaskInstancesState\",\n  \"description\": \"UpdateTaskInstancesState schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_run_id\": {\n      \"description\": \"The task instance's DAG run ID. Either set this or execution_date but not both.\\n\\n*New in version 2.3.0*\\n\",\n      \"type\": \"string\"\n    },\n    \"dry_run\": {\n      \"default\": true,\n      \"description\": \"If set, don't actually run this operation. The response will contain a list of task instances\\nplanned to be affected, but won't be modified in any way.\\n\",\n      \"type\": \"boolean\"\n    },\n    \"execution_date\": {\n      \"description\": \"The execution date. Either set this or dag_run_id but not both.\"\
  ,\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"include_downstream\": {\n      \"description\": \"If set to true, downstream tasks are also affected.\",\n      \"type\": \"boolean\"\n    },\n    \"include_future\": {\n      \"description\": \"If set to True, also tasks from future DAG Runs are affected.\",\n      \"type\": \"boolean\"\n    },\n    \"include_past\": {\n      \"description\": \"If set to True, also tasks from past DAG Runs are affected.\",\n      \"type\": \"boolean\"\n    },\n    \"include_upstream\": {\n      \"description\": \"If set to true, upstream tasks are also affected.\",\n      \"type\": \"boolean\"\n    },\n    \"new_state\": {\n      \"description\": \"Expected new state.\",\n      \"enum\": [\n        \"success\",\n        \"failed\"\n      ],\n      \"type\": \"string\"\n    },\n    \"task_id\": {\n      \"description\": \"The task ID.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-update-task-instances-state-schema.json
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
title: UpdateTaskInstancesState
---
