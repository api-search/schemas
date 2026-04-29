---
description: ''
layout: schema
name: Workflow
properties_list:
- description: Unique workflow instance ID
  name: workflowId
  type: string
- description: Name of the workflow definition
  name: workflowName
  type: string
- description: Version of the workflow definition
  name: workflowVersion
  type: integer
- description: Correlation ID
  name: correlationId
  type: string
- description: Current status of the workflow
  name: status
  type: string
- description: Start time in epoch milliseconds
  name: startTime
  type: integer
- description: End time in epoch milliseconds
  name: endTime
  type: integer
- description: Last update time
  name: updateTime
  type: integer
- description: Workflow input
  name: input
  type: object
- description: Workflow output
  name: output
  type: object
- description: List of tasks in the workflow execution
  name: tasks
  type: array
- description: Reason for failure or termination
  name: reasonForIncompletion
  type: string
- description: List of failed task reference names
  name: failedReferenceTaskNames
  type: array
- description: Workflow priority
  name: priority
  type: integer
- description: Workflow variables
  name: variables
  type: object
- description: Last retry timestamp
  name: lastRetriedTime
  type: integer
- description: Owner application
  name: ownerApp
  type: string
- description: Creation timestamp
  name: createTime
  type: integer
- description: Created by
  name: createdBy
  type: string
- description: Parent workflow ID if this is a sub-workflow
  name: parentWorkflowId
  type: string
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-workflow-schema.json
slug: conductor-conductor-workflow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique workflow instance ID\"\n    },\n    \"workflowName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow definition\"\n    },\n    \"workflowVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"Version of the workflow definition\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the workflow\"\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Start time in epoch milliseconds\"\n    },\n    \"endTime\": {\n      \"type\": \"integer\",\n      \"description\": \"End time in epoch milliseconds\"\n    },\n    \"updateTime\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Last update time\"\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"Workflow input\"\n    },\n    \"output\": {\n      \"type\": \"object\",\n      \"description\": \"Workflow output\"\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"description\": \"List of tasks in the workflow execution\"\n    },\n    \"reasonForIncompletion\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for failure or termination\"\n    },\n    \"failedReferenceTaskNames\": {\n      \"type\": \"array\",\n      \"description\": \"List of failed task reference names\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Workflow priority\"\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"Workflow variables\"\n    },\n    \"lastRetriedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last retry timestamp\"\n   \
  \ },\n    \"ownerApp\": {\n      \"type\": \"string\",\n      \"description\": \"Owner application\"\n    },\n    \"createTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation timestamp\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Created by\"\n    },\n    \"parentWorkflowId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent workflow ID if this is a sub-workflow\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-workflow-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: Workflow
---
