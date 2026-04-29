---
description: ''
layout: schema
name: DescribeWorkflowTypeInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: workflowType
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-describeworkflowtypeinput-schema.json
slug: amazon-swf-describeworkflowtypeinput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"workflowType\"\n  ],\n  \"title\": \"DescribeWorkflowTypeInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain in which this workflow type is registered.\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The workflow type to describe.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-describeworkflowtypeinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DescribeWorkflowTypeInput
---
