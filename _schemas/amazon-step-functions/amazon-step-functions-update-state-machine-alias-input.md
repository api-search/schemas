---
description: UpdateStateMachineAliasInput schema from Amazon Step Functions API
layout: schema
name: UpdateStateMachineAliasInput
properties_list:
- description: ''
  name: stateMachineAliasArn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: routingConfiguration
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-update-state-machine-alias-input-schema.json
slug: amazon-step-functions-update-state-machine-alias-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-state-machine-alias-input-schema.json\",\n  \"title\": \"UpdateStateMachineAliasInput\",\n  \"description\": \"UpdateStateMachineAliasInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine alias.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasDescription\"\n        },\n        {\n          \"description\": \"A description of the state machine alias.\"\n        }\n      ]\n    },\n    \"routingConfiguration\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/RoutingConfigurationList\"\n        },\n        {\n          \"description\": \"<p>The routing configuration of the state machine alias.</p> <p>An array of <code>RoutingConfig</code> objects that specifies up to two state machine versions that the alias starts executions for.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineAliasArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-state-machine-alias-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: UpdateStateMachineAliasInput
---
