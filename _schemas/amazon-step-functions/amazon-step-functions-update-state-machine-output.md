---
description: UpdateStateMachineOutput schema from Amazon Step Functions API
layout: schema
name: UpdateStateMachineOutput
properties_list:
- description: ''
  name: updateDate
  type: object
- description: ''
  name: revisionId
  type: object
- description: ''
  name: stateMachineVersionArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-update-state-machine-output-schema.json
slug: amazon-step-functions-update-state-machine-output
source_filename: amazon-step-functions-update-state-machine-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-state-machine-output-schema.json\",\n  \"title\": \"UpdateStateMachineOutput\",\n  \"description\": \"UpdateStateMachineOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time the state machine was updated.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \"The revision identifier for the updated state machine.\"\n        }\n      ]\n    },\n    \"stateMachineVersionArn\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the published state machine version.</p> <p>If the <code>publish</code> parameter isn't set to <code>true</code>, this field returns null.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"updateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-state-machine-output-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: UpdateStateMachineOutput
---
