---
description: CreateStateMachineAliasOutput schema from Amazon Step Functions API
layout: schema
name: CreateStateMachineAliasOutput
properties_list:
- description: ''
  name: stateMachineAliasArn
  type: object
- description: ''
  name: creationDate
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-create-state-machine-alias-output-schema.json
slug: amazon-step-functions-create-state-machine-alias-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-create-state-machine-alias-output-schema.json\",\n  \"title\": \"CreateStateMachineAliasOutput\",\n  \"description\": \"CreateStateMachineAliasOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the created state machine alias.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the state machine alias was created.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  stateMachineAliasArn\",\n    \"creationDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-create-state-machine-alias-output-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: CreateStateMachineAliasOutput
---
