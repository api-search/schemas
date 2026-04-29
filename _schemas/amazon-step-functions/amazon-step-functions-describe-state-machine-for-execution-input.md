---
description: DescribeStateMachineForExecutionInput schema from Amazon Step Functions API
layout: schema
name: DescribeStateMachineForExecutionInput
properties_list:
- description: ''
  name: executionArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-state-machine-for-execution-input-schema.json
slug: amazon-step-functions-describe-state-machine-for-execution-input
source_filename: amazon-step-functions-describe-state-machine-for-execution-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-for-execution-input-schema.json\",\n  \"title\": \"DescribeStateMachineForExecutionInput\",\n  \"description\": \"DescribeStateMachineForExecutionInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the execution you want state machine information for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"executionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-for-execution-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeStateMachineForExecutionInput
---
