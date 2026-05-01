---
description: CreateStateMachineOutput schema from Amazon Step Functions API
layout: schema
name: CreateStateMachineOutput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: stateMachineVersionArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-create-state-machine-output-schema.json
slug: amazon-step-functions-create-state-machine-output
source_filename: amazon-step-functions-create-state-machine-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-create-state-machine-output-schema.json\",\n  \"title\": \"CreateStateMachineOutput\",\n  \"description\": \"CreateStateMachineOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the created state machine.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the state machine is created.\"\n        }\n      ]\n    },\n    \"stateMachineVersionArn\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the created state machine version. If you do not set the <code>publish</code> parameter to <code>true</code>, this field returns null value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineArn\",\n    \"creationDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-create-state-machine-output-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: CreateStateMachineOutput
---
