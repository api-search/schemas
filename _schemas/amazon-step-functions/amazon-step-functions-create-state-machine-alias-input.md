---
description: CreateStateMachineAliasInput schema from Amazon Step Functions API
layout: schema
name: CreateStateMachineAliasInput
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: routingConfiguration
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-create-state-machine-alias-input-schema.json
slug: amazon-step-functions-create-state-machine-alias-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-create-state-machine-alias-input-schema.json\",\n  \"title\": \"CreateStateMachineAliasInput\",\n  \"description\": \"CreateStateMachineAliasInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasDescription\"\n        },\n        {\n          \"description\": \"A description for the state machine alias.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CharacterRestrictedName\"\n        },\n        {\n          \"description\": \"<p>The name of the state machine alias.</p> <p>To avoid conflict with version ARNs, don't use an integer in the name of the alias.</p>\"\
  \n        }\n      ]\n    },\n    \"routingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoutingConfigurationList\"\n        },\n        {\n          \"description\": \"The routing configuration of a state machine alias. The routing configuration shifts execution traffic between two state machine versions. <code>routingConfiguration</code> contains an array of <code>RoutingConfig</code> objects that specify up to two state machine versions. Step Functions then randomly choses which version to run an execution with based on the weight assigned to each <code>RoutingConfig</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"routingConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-create-state-machine-alias-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: CreateStateMachineAliasInput
---
