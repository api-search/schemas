---
description: ''
layout: schema
name: RequestCancelWorkflowExecutionInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: workflowId
  type: object
- description: ''
  name: runId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-requestcancelworkflowexecutioninput-schema.json
slug: amazon-swf-requestcancelworkflowexecutioninput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"workflowId\"\n  ],\n  \"title\": \"RequestCancelWorkflowExecutionInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain containing the workflow execution to cancel.\"\n        }\n      ]\n    },\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The workflowId of the workflow execution to cancel.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunIdOptional\"\n        },\n        {\n          \"description\": \"The runId of the workflow execution to cancel.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-requestcancelworkflowexecutioninput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: RequestCancelWorkflowExecutionInput
---
