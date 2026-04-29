---
description: Represents a workflow execution.
layout: schema
name: WorkflowExecution
properties_list:
- description: ''
  name: workflowId
  type: object
- description: ''
  name: runId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecution-schema.json
slug: amazon-swf-workflowexecution
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowId\",\n    \"runId\"\n  ],\n  \"properties\": {\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The user defined identifier associated with the workflow execution.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunId\"\n        },\n        {\n          \"description\": \"A system-generated unique identifier for the workflow execution.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents a workflow execution.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecution\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecution-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecution
---
