---
description: A task run executing a standalone task or a DAG of tasks starting from the root task.
layout: schema
name: TaskRun
properties_list:
- description: The name of the root task in the current task run.
  name: root_task_name
  type: string
- description: The name of the current database for the task run.
  name: database_name
  type: string
- description: The name of the current schema for the task run.
  name: schema_name
  type: string
- description: The current state of the task run.
  name: state
  type: string
- description: The name of the first task throwing an error in the task run.
  name: first_error_task_name
  type: string
- description: The first error code thrown in the task run.
  name: first_error_code
  type: integer
- description: The first error message thrown in the task run.
  name: first_error_message
  type: string
- description: The scheduled time for the task run.
  name: scheduled_time
  type: string
- description: The start time for the task run query.
  name: query_start_time
  type: string
- description: The next upcoming time for the task run.
  name: next_scheduled_time
  type: string
- description: The time this task run was last completed.
  name: completed_time
  type: string
- description: The unique task ID for the root task.
  name: root_task_id
  type: string
- description: The current version of the DAG on the task run.
  name: graph_version
  type: integer
- description: The unique ID for the current task run.
  name: run_id
  type: integer
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/task-task-run-schema.json
slug: task-task-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskRun\",\n  \"type\": \"object\",\n  \"description\": \"A task run executing a standalone task or a DAG of tasks starting from the root task.\",\n  \"properties\": {\n    \"root_task_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the root task in the current task run.\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the current database for the task run.\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the current schema for the task run.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the task run.\"\n    },\n    \"first_error_task_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the first task throwing an error in the task run.\"\n    },\n    \"first_error_code\": {\n   \
  \   \"type\": \"integer\",\n      \"description\": \"The first error code thrown in the task run.\"\n    },\n    \"first_error_message\": {\n      \"type\": \"string\",\n      \"description\": \"The first error message thrown in the task run.\"\n    },\n    \"scheduled_time\": {\n      \"type\": \"string\",\n      \"description\": \"The scheduled time for the task run.\"\n    },\n    \"query_start_time\": {\n      \"type\": \"string\",\n      \"description\": \"The start time for the task run query.\"\n    },\n    \"next_scheduled_time\": {\n      \"type\": \"string\",\n      \"description\": \"The next upcoming time for the task run.\"\n    },\n    \"completed_time\": {\n      \"type\": \"string\",\n      \"description\": \"The time this task run was last completed.\"\n    },\n    \"root_task_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique task ID for the root task.\"\n    },\n    \"graph_version\": {\n      \"type\": \"integer\",\n      \"description\": \"The\
  \ current version of the DAG on the task run.\"\n    },\n    \"run_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique ID for the current task run.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/task-task-run-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: TaskRun
---
