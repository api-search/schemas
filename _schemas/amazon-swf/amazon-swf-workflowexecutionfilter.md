---
description: Used to filter the workflow executions in visibility APIs by their <code>workflowId</code>.
layout: schema
name: WorkflowExecutionFilter
properties_list:
- description: ''
  name: workflowId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutionfilter-schema.json
slug: amazon-swf-workflowexecutionfilter
source_filename: amazon-swf-workflowexecutionfilter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowId\"\n  ],\n  \"properties\": {\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The workflowId to pass of match the criteria of this filter.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Used to filter the workflow executions in visibility APIs by their <code>workflowId</code>.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionFilter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutionfilter-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: WorkflowExecutionFilter
---
