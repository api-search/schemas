---
description: Contains details about a specific state machine alias.
layout: schema
name: StateMachineAliasListItem
properties_list:
- description: ''
  name: stateMachineAliasArn
  type: object
- description: ''
  name: creationDate
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-state-machine-alias-list-item-schema.json
slug: amazon-step-functions-state-machine-alias-list-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-state-machine-alias-list-item-schema.json\",\n  \"title\": \"StateMachineAliasListItem\",\n  \"description\": \"Contains details about a specific state machine alias.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies a state machine alias. The alias ARN is a combination of state machine ARN and the alias name separated by a colon (:). For example, <code>stateMachineARN:PROD</code>.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\"\
  : \"The creation date of a state machine alias.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineAliasArn\",\n    \"creationDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-state-machine-alias-list-item-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: StateMachineAliasListItem
---
