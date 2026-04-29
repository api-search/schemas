---
description: ClearTaskInstances schema from Apache Airflow API
layout: schema
name: ClearTaskInstances
properties_list:
- description: The DagRun ID for this task instance
  name: dag_run_id
  type: string
- description: If set, don't actually run this operation. The response will contain a list of task instances planned to be cleaned, but not modified in any way.
  name: dry_run
  type: boolean
- description: The maximum execution date to clear.
  name: end_date
  type: string
- description: If set to true, downstream tasks are also affected.
  name: include_downstream
  type: boolean
- description: If set to True, also tasks from future DAG Runs are affected.
  name: include_future
  type: boolean
- description: Clear tasks in the parent dag of the subdag.
  name: include_parentdag
  type: boolean
- description: If set to True, also tasks from past DAG Runs are affected.
  name: include_past
  type: boolean
- description: Clear tasks in subdags and clear external tasks indicated by ExternalTaskMarker.
  name: include_subdags
  type: boolean
- description: If set to true, upstream tasks are also affected.
  name: include_upstream
  type: boolean
- description: Only clear failed tasks.
  name: only_failed
  type: boolean
- description: Only clear running tasks.
  name: only_running
  type: boolean
- description: Set state of DAG runs to RUNNING.
  name: reset_dag_runs
  type: boolean
- description: The minimum execution date to clear.
  name: start_date
  type: string
- description: A list of task ids to clear. *New in version 2.1.0*
  name: task_ids
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-clear-task-instances-schema.json
slug: openapi.yaml-clear-task-instances
source_filename: openapi.yaml-clear-task-instances-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-clear-task-instances-schema.json\",\n  \"title\": \"ClearTaskInstances\",\n  \"description\": \"ClearTaskInstances schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_run_id\": {\n      \"description\": \"The DagRun ID for this task instance\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"dry_run\": {\n      \"default\": true,\n      \"description\": \"If set, don't actually run this operation. The response will contain a list of task instances\\nplanned to be cleaned, but not modified in any way.\\n\",\n      \"type\": \"boolean\"\n    },\n    \"end_date\": {\n      \"description\": \"The maximum execution date to clear.\",\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"include_downstream\": {\n  \
  \    \"default\": false,\n      \"description\": \"If set to true, downstream tasks are also affected.\",\n      \"type\": \"boolean\"\n    },\n    \"include_future\": {\n      \"default\": false,\n      \"description\": \"If set to True, also tasks from future DAG Runs are affected.\",\n      \"type\": \"boolean\"\n    },\n    \"include_parentdag\": {\n      \"description\": \"Clear tasks in the parent dag of the subdag.\",\n      \"type\": \"boolean\"\n    },\n    \"include_past\": {\n      \"default\": false,\n      \"description\": \"If set to True, also tasks from past DAG Runs are affected.\",\n      \"type\": \"boolean\"\n    },\n    \"include_subdags\": {\n      \"description\": \"Clear tasks in subdags and clear external tasks indicated by ExternalTaskMarker.\",\n      \"type\": \"boolean\"\n    },\n    \"include_upstream\": {\n      \"default\": false,\n      \"description\": \"If set to true, upstream tasks are also affected.\",\n      \"type\": \"boolean\"\n    },\n    \"only_failed\"\
  : {\n      \"default\": true,\n      \"description\": \"Only clear failed tasks.\",\n      \"type\": \"boolean\"\n    },\n    \"only_running\": {\n      \"default\": false,\n      \"description\": \"Only clear running tasks.\",\n      \"type\": \"boolean\"\n    },\n    \"reset_dag_runs\": {\n      \"description\": \"Set state of DAG runs to RUNNING.\",\n      \"type\": \"boolean\"\n    },\n    \"start_date\": {\n      \"description\": \"The minimum execution date to clear.\",\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"task_ids\": {\n      \"description\": \"A list of task ids to clear.\\n\\n*New in version 2.1.0*\\n\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-clear-task-instances-schema.json
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
title: ClearTaskInstances
---
