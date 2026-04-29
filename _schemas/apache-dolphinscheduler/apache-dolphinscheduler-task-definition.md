---
description: A task node in a DolphinScheduler workflow definition DAG.
layout: schema
name: TaskDefinition
properties_list:
- description: Task definition ID.
  name: id
  type: integer
- description: Globally unique task code.
  name: code
  type: integer
- description: Task name within the workflow.
  name: name
  type: string
- description: Task execution type.
  name: taskType
  type: string
- description: Task-specific parameters (structure varies by taskType).
  name: taskParams
  type: object
- description: Task description.
  name: description
  type: string
- description: Whether this task is enabled.
  name: flag
  type: string
- description: Task priority for scheduling.
  name: taskPriority
  type: string
- description: Worker group this task should run on.
  name: workerGroup
  type: string
- description: Number of retry attempts on failure.
  name: retryTimes
  type: integer
- description: Interval in minutes between retry attempts.
  name: retryInterval
  type: integer
- description: Task execution timeout in minutes.
  name: timeout
  type: integer
provider_name: Apache DolphinScheduler
provider_slug: apache-dolphinscheduler
schema_file: json-schema/apache-dolphinscheduler-task-definition-schema.json
slug: apache-dolphinscheduler-task-definition
source_filename: apache-dolphinscheduler-task-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dolphinscheduler/refs/heads/main/json-schema/apache-dolphinscheduler-task-definition-schema.json\",\n  \"title\": \"TaskDefinition\",\n  \"description\": \"A task node in a DolphinScheduler workflow definition DAG.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Task definition ID.\",\n      \"example\": 2001\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Globally unique task code.\",\n      \"example\": 9999999999999\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Task name within the workflow.\",\n      \"example\": \"extract-sales-data\"\n    },\n    \"taskType\": {\n      \"type\": \"string\",\n      \"description\": \"Task execution type.\",\n      \"enum\": [\n        \"SHELL\",\n        \"SQL\",\n\
  \        \"SPARK\",\n        \"FLINK\",\n        \"PYTHON\",\n        \"HTTP\",\n        \"DATAX\",\n        \"SEATUNNEL\",\n        \"JUPYTER\",\n        \"PYTORCH\",\n        \"CONDITIONS\",\n        \"SWITCH\",\n        \"SUB_PROCESS\",\n        \"DEPENDENT\"\n      ],\n      \"example\": \"SPARK\"\n    },\n    \"taskParams\": {\n      \"type\": \"object\",\n      \"description\": \"Task-specific parameters (structure varies by taskType).\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Task description.\",\n      \"example\": \"Extract daily sales data from source database\"\n    },\n    \"flag\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this task is enabled.\",\n      \"enum\": [\n        \"YES\",\n        \"NO\"\n      ],\n      \"default\": \"YES\",\n      \"example\": \"YES\"\n    },\n    \"taskPriority\": {\n      \"type\": \"string\",\n      \"description\": \"Task priority for scheduling.\",\n      \"enum\": [\n\
  \        \"HIGHEST\",\n        \"HIGH\",\n        \"MEDIUM\",\n        \"LOW\",\n        \"LOWEST\"\n      ],\n      \"example\": \"MEDIUM\"\n    },\n    \"workerGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Worker group this task should run on.\",\n      \"default\": \"default\",\n      \"example\": \"default\"\n    },\n    \"retryTimes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of retry attempts on failure.\",\n      \"minimum\": 0,\n      \"default\": 0,\n      \"example\": 3\n    },\n    \"retryInterval\": {\n      \"type\": \"integer\",\n      \"description\": \"Interval in minutes between retry attempts.\",\n      \"default\": 1,\n      \"example\": 5\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Task execution timeout in minutes.\",\n      \"default\": 0,\n      \"example\": 30\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"taskType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dolphinscheduler/refs/heads/main/json-schema/apache-dolphinscheduler-task-definition-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: TaskDefinition
---
