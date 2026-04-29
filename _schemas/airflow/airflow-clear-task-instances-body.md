---
description: Request body for Clear Task Instances endpoint.
layout: schema
name: ClearTaskInstancesBody
properties_list:
- description: ''
  name: dry_run
  type: boolean
- description: ''
  name: start_date
  type: object
- description: ''
  name: end_date
  type: object
- description: ''
  name: only_failed
  type: boolean
- description: ''
  name: only_running
  type: boolean
- description: ''
  name: reset_dag_runs
  type: boolean
- description: A list of `task_id` or [`task_id`, `map_index`]. If only the `task_id` is provided for a mapped task, all of its map indices will be targeted.
  name: task_ids
  type: object
- description: ''
  name: dag_run_id
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
- description: (Experimental) Run on the latest bundle version of the dag after clearing the task instances.
  name: run_on_latest_version
  type: boolean
- description: ''
  name: prevent_running_task
  type: boolean
- description: ''
  name: note
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-clear-task-instances-body-schema.json
slug: airflow-clear-task-instances-body
source_filename: airflow-clear-task-instances-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-clear-task-instances-body-schema.json\",\n  \"title\": \"ClearTaskInstancesBody\",\n  \"description\": \"Request body for Clear Task Instances endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dry_run\": {\n      \"type\": \"boolean\",\n      \"title\": \"Dry Run\",\n      \"default\": true\n    },\n    \"start_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Start Date\"\n    },\n    \"end_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date\"\n    },\n    \"only_failed\": {\n\
  \      \"type\": \"boolean\",\n      \"title\": \"Only Failed\",\n      \"default\": true\n    },\n    \"only_running\": {\n      \"type\": \"boolean\",\n      \"title\": \"Only Running\",\n      \"default\": false\n    },\n    \"reset_dag_runs\": {\n      \"type\": \"boolean\",\n      \"title\": \"Reset Dag Runs\",\n      \"default\": true\n    },\n    \"task_ids\": {\n      \"anyOf\": [\n        {\n          \"items\": {\n            \"anyOf\": [\n              {\n                \"type\": \"string\"\n              },\n              {\n                \"prefixItems\": [\n                  {\n                    \"type\": \"string\"\n                  },\n                  {\n                    \"type\": \"integer\"\n                  }\n                ],\n                \"type\": \"array\",\n                \"maxItems\": 2,\n                \"minItems\": 2\n              }\n            ]\n          },\n          \"type\": \"array\"\n        },\n        {\n          \"type\": \"null\"\
  \n        }\n      ],\n      \"title\": \"Task Ids\",\n      \"description\": \"A list of `task_id` or [`task_id`, `map_index`]. If only the `task_id` is provided for a mapped task, all of its map indices will be targeted.\"\n    },\n    \"dag_run_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Dag Run Id\"\n    },\n    \"include_upstream\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Upstream\",\n      \"default\": false\n    },\n    \"include_downstream\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Downstream\",\n      \"default\": false\n    },\n    \"include_future\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Future\",\n      \"default\": false\n    },\n    \"include_past\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Past\",\n      \"default\": false\n    },\n    \"run_on_latest_version\": {\n      \"\
  type\": \"boolean\",\n      \"title\": \"Run On Latest Version\",\n      \"description\": \"(Experimental) Run on the latest bundle version of the dag after clearing the task instances.\",\n      \"default\": false\n    },\n    \"prevent_running_task\": {\n      \"type\": \"boolean\",\n      \"title\": \"Prevent Running Task\",\n      \"default\": false\n    },\n    \"note\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"maxLength\": 1000\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Note\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-clear-task-instances-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ClearTaskInstancesBody
---
