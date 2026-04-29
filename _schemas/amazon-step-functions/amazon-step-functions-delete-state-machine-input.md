---
description: DeleteStateMachineInput schema from Amazon Step Functions API
layout: schema
name: DeleteStateMachineInput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-delete-state-machine-input-schema.json
slug: amazon-step-functions-delete-state-machine-input
source_filename: amazon-step-functions-delete-state-machine-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-delete-state-machine-input-schema.json\",\n  \"title\": \"DeleteStateMachineInput\",\n  \"description\": \"DeleteStateMachineInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-delete-state-machine-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: DeleteStateMachineInput
---
