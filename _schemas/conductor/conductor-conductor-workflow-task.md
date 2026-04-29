---
description: ''
layout: schema
name: WorkflowTask
properties_list:
- description: Name of the task
  name: name
  type: string
- description: Unique reference name for the task within the workflow
  name: taskReferenceName
  type: string
- description: The type of task
  name: type
  type: string
- description: Task description
  name: description
  type: string
- description: Input parameter mappings
  name: inputParameters
  type: object
- description: Whether this task is optional
  name: optional
  type: boolean
- description: Delay in seconds before starting the task
  name: startDelay
  type: integer
- description: Whether the task is completed asynchronously
  name: asyncComplete
  type: boolean
- description: Number of retries
  name: retryCount
  type: integer
- description: Sink for EVENT tasks
  name: sink
  type: string
- description: Sub workflow parameters
  name: subWorkflowParam
  type: object
- description: List of task reference names to join on
  name: joinOn
  type: array
- description: List of forked task lists
  name: forkTasks
  type: array
- description: Decision cases for SWITCH/DECISION tasks
  name: decisionCases
  type: object
- description: Default case tasks for SWITCH/DECISION
  name: defaultCase
  type: array
- description: Loop condition for DO_WHILE tasks
  name: loopCondition
  type: string
- description: Tasks to loop over in DO_WHILE
  name: loopOver
  type: array
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-workflow-task-schema.json
slug: conductor-conductor-workflow-task
source_filename: conductor-conductor-workflow-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowTask\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the task\"\n    },\n    \"taskReferenceName\": {\n      \"type\": \"string\",\n      \"description\": \"Unique reference name for the task within the workflow\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of task\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Task description\"\n    },\n    \"inputParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameter mappings\"\n    },\n    \"optional\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this task is optional\"\n    },\n    \"startDelay\": {\n      \"type\": \"integer\",\n      \"description\": \"Delay in seconds before starting the task\"\n    },\n    \"asyncComplete\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the task is completed asynchronously\"\n    },\n    \"retryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of retries\"\n    },\n    \"sink\": {\n      \"type\": \"string\",\n      \"description\": \"Sink for EVENT tasks\"\n    },\n    \"subWorkflowParam\": {\n      \"type\": \"object\",\n      \"description\": \"Sub workflow parameters\"\n    },\n    \"joinOn\": {\n      \"type\": \"array\",\n      \"description\": \"List of task reference names to join on\"\n    },\n    \"forkTasks\": {\n      \"type\": \"array\",\n      \"description\": \"List of forked task lists\"\n    },\n    \"decisionCases\": {\n      \"type\": \"object\",\n      \"description\": \"Decision cases for SWITCH/DECISION tasks\"\n    },\n    \"defaultCase\": {\n      \"type\": \"array\",\n      \"description\": \"Default case tasks for SWITCH/DECISION\"\n    },\n    \"loopCondition\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Loop condition for DO_WHILE tasks\"\n    },\n    \"loopOver\": {\n      \"type\": \"array\",\n      \"description\": \"Tasks to loop over in DO_WHILE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-workflow-task-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: WorkflowTask
---
