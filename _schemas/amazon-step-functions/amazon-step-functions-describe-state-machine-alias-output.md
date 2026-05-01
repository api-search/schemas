---
description: DescribeStateMachineAliasOutput schema from Amazon Step Functions API
layout: schema
name: DescribeStateMachineAliasOutput
properties_list:
- description: ''
  name: stateMachineAliasArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: routingConfiguration
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: updateDate
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-state-machine-alias-output-schema.json
slug: amazon-step-functions-describe-state-machine-alias-output
source_filename: amazon-step-functions-describe-state-machine-alias-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-alias-output-schema.json\",\n  \"title\": \"DescribeStateMachineAliasOutput\",\n  \"description\": \"DescribeStateMachineAliasOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine alias.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the state machine alias.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/AliasDescription\"\n        },\n        {\n          \"description\": \"A description of the alias.\"\n        }\n      ]\n    },\n    \"routingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoutingConfigurationList\"\n        },\n        {\n          \"description\": \"The routing configuration of the alias.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the state machine alias was created.\"\n        }\n      ]\n    },\n    \"updateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The date the state machine alias was last updated.</p> <p>For a newly created state machine, this is the same as the creation date.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-alias-output-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeStateMachineAliasOutput
---
