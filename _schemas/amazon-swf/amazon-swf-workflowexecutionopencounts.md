---
description: Contains the counts of open tasks, child workflow executions and timers for a workflow execution.
layout: schema
name: WorkflowExecutionOpenCounts
properties_list:
- description: ''
  name: openActivityTasks
  type: object
- description: ''
  name: openDecisionTasks
  type: object
- description: ''
  name: openTimers
  type: object
- description: ''
  name: openChildWorkflowExecutions
  type: object
- description: ''
  name: openLambdaFunctions
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutionopencounts-schema.json
slug: amazon-swf-workflowexecutionopencounts
source_filename: amazon-swf-workflowexecutionopencounts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"openActivityTasks\",\n    \"openDecisionTasks\",\n    \"openTimers\",\n    \"openChildWorkflowExecutions\"\n  ],\n  \"properties\": {\n    \"openActivityTasks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The count of activity tasks whose status is <code>OPEN</code>.\"\n        }\n      ]\n    },\n    \"openDecisionTasks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenDecisionTasksCount\"\n        },\n        {\n          \"description\": \"The count of decision tasks whose status is OPEN. A workflow execution can have at most one open decision task.\"\n        }\n      ]\n    },\n    \"openTimers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The count of timers started by this workflow execution that\
  \ have not fired yet.\"\n        }\n      ]\n    },\n    \"openChildWorkflowExecutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The count of child workflow executions whose status is <code>OPEN</code>.\"\n        }\n      ]\n    },\n    \"openLambdaFunctions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The count of Lambda tasks whose status is <code>OPEN</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains the counts of open tasks, child workflow executions and timers for a workflow execution.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionOpenCounts\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutionopencounts-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: WorkflowExecutionOpenCounts
---
