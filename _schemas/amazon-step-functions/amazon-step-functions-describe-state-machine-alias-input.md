---
description: DescribeStateMachineAliasInput schema from Amazon Step Functions API
layout: schema
name: DescribeStateMachineAliasInput
properties_list:
- description: ''
  name: stateMachineAliasArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-state-machine-alias-input-schema.json
slug: amazon-step-functions-describe-state-machine-alias-input
source_filename: amazon-step-functions-describe-state-machine-alias-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-alias-input-schema.json\",\n  \"title\": \"DescribeStateMachineAliasInput\",\n  \"description\": \"DescribeStateMachineAliasInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine alias.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineAliasArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-alias-input-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeStateMachineAliasInput
---
