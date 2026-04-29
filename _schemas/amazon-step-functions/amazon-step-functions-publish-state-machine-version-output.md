---
description: PublishStateMachineVersionOutput schema from Amazon Step Functions API
layout: schema
name: PublishStateMachineVersionOutput
properties_list:
- description: ''
  name: creationDate
  type: object
- description: ''
  name: stateMachineVersionArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-publish-state-machine-version-output-schema.json
slug: amazon-step-functions-publish-state-machine-version-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-publish-state-machine-version-output-schema.json\",\n  \"title\": \"PublishStateMachineVersionOutput\",\n  \"description\": \"PublishStateMachineVersionOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the version was created.\"\n        }\n      ]\n    },\n    \"stateMachineVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) (ARN) that identifies the state machine version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  creationDate\",\n    \"stateMachineVersionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-publish-state-machine-version-output-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: PublishStateMachineVersionOutput
---
