---
description: Contains details about a workflow execution.
layout: schema
name: WorkflowExecutionDetail
properties_list:
- description: ''
  name: executionInfo
  type: object
- description: ''
  name: executionConfiguration
  type: object
- description: ''
  name: openCounts
  type: object
- description: ''
  name: latestActivityTaskTimestamp
  type: object
- description: ''
  name: latestExecutionContext
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutiondetail-schema.json
slug: amazon-swf-workflowexecutiondetail
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"executionInfo\",\n    \"executionConfiguration\",\n    \"openCounts\"\n  ],\n  \"properties\": {\n    \"executionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionInfo\"\n        },\n        {\n          \"description\": \"Information about the workflow execution.\"\n        }\n      ]\n    },\n    \"executionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionConfiguration\"\n        },\n        {\n          \"description\": \"The configuration settings for this workflow execution including timeout values, tasklist etc.\"\n        }\n      ]\n    },\n    \"openCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionOpenCounts\"\n        },\n        {\n          \"description\": \"The number of tasks for this workflow execution. This includes open and closed tasks of\
  \ all types.\"\n        }\n      ]\n    },\n    \"latestActivityTaskTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the last activity task was scheduled for this workflow execution. You can use this information to determine if the workflow has not made progress for an unusually long period of time and might require a corrective action.\"\n        }\n      ]\n    },\n    \"latestExecutionContext\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The latest executionContext provided by the decider for this workflow execution. A decider can provide an executionContext (a free-form string) when closing a decision task using <a>RespondDecisionTaskCompleted</a>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains details about a workflow execution.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\
  ,\n  \"title\": \"WorkflowExecutionDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutiondetail-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecutionDetail
---
