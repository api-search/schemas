---
description: Request body for bulk update, and delete task instances.
layout: schema
name: BulkTaskInstanceBody
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
- description: ''
  name: task_id
  type: string
- description: ''
  name: map_index
  type: object
- description: ''
  name: dag_id
  type: object
- description: ''
  name: dag_run_id
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-bulk-task-instance-body-schema.json
slug: airflow-bulk-task-instance-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-task-instance-body-schema.json\",\n  \"title\": \"BulkTaskInstanceBody\",\n  \"description\": \"Request body for bulk update, and delete task instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"new_state\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskInstanceState\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    },\n    \"note\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"maxLength\": 1000\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Note\"\n    },\n    \"include_upstream\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Upstream\",\n      \"default\": false\n    },\n    \"include_downstream\": {\n      \"type\": \"boolean\"\
  ,\n      \"title\": \"Include Downstream\",\n      \"default\": false\n    },\n    \"include_future\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Future\",\n      \"default\": false\n    },\n    \"include_past\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Past\",\n      \"default\": false\n    },\n    \"task_id\": {\n      \"type\": \"string\",\n      \"title\": \"Task Id\"\n    },\n    \"map_index\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Map Index\"\n    },\n    \"dag_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Dag Id\"\n    },\n    \"dag_run_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Dag Run\
  \ Id\"\n    }\n  },\n  \"required\": [\n    \"task_id\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-task-instance-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BulkTaskInstanceBody
---
