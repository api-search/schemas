---
description: A running or completed instance of a workflow definition in Apache DolphinScheduler.
layout: schema
name: WorkflowInstance
properties_list:
- description: Unique workflow instance ID.
  name: id
  type: integer
- description: Code of the workflow definition that created this instance.
  name: processDefinitionCode
  type: integer
- description: Workflow instance name (typically includes a timestamp).
  name: name
  type: string
- description: Execution state of this workflow instance.
  name: state
  type: string
- description: Execution start time.
  name: startTime
  type: string
- description: Execution end time (null if still running).
  name: endTime
  type: string
- description: Human-readable execution duration.
  name: duration
  type: string
- description: Number of times this instance has been re-run.
  name: runTimes
  type: integer
- description: Type of command that triggered this instance.
  name: commandType
  type: string
- description: Worker host that is executing this instance.
  name: host
  type: string
provider_name: Apache DolphinScheduler
provider_slug: apache-dolphinscheduler
schema_file: json-schema/apache-dolphinscheduler-workflow-instance-schema.json
slug: apache-dolphinscheduler-workflow-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dolphinscheduler/refs/heads/main/json-schema/apache-dolphinscheduler-workflow-instance-schema.json\",\n  \"title\": \"WorkflowInstance\",\n  \"description\": \"A running or completed instance of a workflow definition in Apache DolphinScheduler.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique workflow instance ID.\",\n      \"example\": 500123\n    },\n    \"processDefinitionCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Code of the workflow definition that created this instance.\",\n      \"example\": 8888888888888\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Workflow instance name (typically includes a timestamp).\",\n      \"example\": \"daily-etl-pipeline-20250315\"\n    },\n    \"state\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Execution state of this workflow instance.\",\n      \"enum\": [\n        \"SUBMITTED_SUCCESS\",\n        \"RUNNING_EXECUTION\",\n        \"PAUSE\",\n        \"STOP\",\n        \"FAILURE\",\n        \"SUCCESS\",\n        \"NEED_FAULT_TOLERANCE\",\n        \"KILL\",\n        \"WAITING_THREAD\",\n        \"WAITING_DEPEND\",\n        \"DELAY_EXECUTION\",\n        \"FORCED_SUCCESS\",\n        \"SERIAL_WAIT\"\n      ],\n      \"example\": \"RUNNING_EXECUTION\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Execution start time.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Execution end time (null if still running).\",\n      \"example\": \"2025-03-15T15:00:00Z\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable execution\
  \ duration.\",\n      \"example\": \"30m 0s\"\n    },\n    \"runTimes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times this instance has been re-run.\",\n      \"example\": 1\n    },\n    \"commandType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of command that triggered this instance.\",\n      \"example\": \"START_PROCESS\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Worker host that is executing this instance.\",\n      \"example\": \"worker-01:1234\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dolphinscheduler/refs/heads/main/json-schema/apache-dolphinscheduler-workflow-instance-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: WorkflowInstance
---
