---
description: Contains details about a specific state machine version.
layout: schema
name: StateMachineVersionListItem
properties_list:
- description: ''
  name: stateMachineVersionArn
  type: object
- description: ''
  name: creationDate
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-state-machine-version-list-item-schema.json
slug: amazon-step-functions-state-machine-version-list-item
source_filename: amazon-step-functions-state-machine-version-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-state-machine-version-list-item-schema.json\",\n  \"title\": \"StateMachineVersionListItem\",\n  \"description\": \"Contains details about a specific state machine version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies a state machine version. The version ARN is a combination of state machine ARN and the version number separated by a colon (:). For example, <code>stateMachineARN:1</code>.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n   \
  \       \"description\": \"The creation date of a state machine version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineVersionArn\",\n    \"creationDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-state-machine-version-list-item-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: StateMachineVersionListItem
---
