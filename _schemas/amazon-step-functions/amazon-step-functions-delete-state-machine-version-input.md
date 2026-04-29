---
description: DeleteStateMachineVersionInput schema from Amazon Step Functions API
layout: schema
name: DeleteStateMachineVersionInput
properties_list:
- description: ''
  name: stateMachineVersionArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-delete-state-machine-version-input-schema.json
slug: amazon-step-functions-delete-state-machine-version-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-delete-state-machine-version-input-schema.json\",\n  \"title\": \"DeleteStateMachineVersionInput\",\n  \"description\": \"DeleteStateMachineVersionInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine version to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineVersionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-delete-state-machine-version-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: DeleteStateMachineVersionInput
---
