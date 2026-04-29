---
description: ''
layout: schema
name: DescribeWorkflowExecutionInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: execution
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-describeworkflowexecutioninput-schema.json
slug: amazon-swf-describeworkflowexecutioninput
source_filename: amazon-swf-describeworkflowexecutioninput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"execution\"\n  ],\n  \"title\": \"DescribeWorkflowExecutionInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain containing the workflow execution.\"\n        }\n      ]\n    },\n    \"execution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"The workflow execution to describe.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-describeworkflowexecutioninput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DescribeWorkflowExecutionInput
---
