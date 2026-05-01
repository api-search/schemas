---
description: UpdateStateMachineAliasOutput schema from Amazon Step Functions API
layout: schema
name: UpdateStateMachineAliasOutput
properties_list:
- description: ''
  name: updateDate
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-update-state-machine-alias-output-schema.json
slug: amazon-step-functions-update-state-machine-alias-output
source_filename: amazon-step-functions-update-state-machine-alias-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-state-machine-alias-output-schema.json\",\n  \"title\": \"UpdateStateMachineAliasOutput\",\n  \"description\": \"UpdateStateMachineAliasOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time the state machine alias was updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"updateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-state-machine-alias-output-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: UpdateStateMachineAliasOutput
---
