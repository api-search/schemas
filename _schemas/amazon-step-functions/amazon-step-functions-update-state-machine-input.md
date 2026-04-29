---
description: UpdateStateMachineInput schema from Amazon Step Functions API
layout: schema
name: UpdateStateMachineInput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: definition
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: loggingConfiguration
  type: object
- description: ''
  name: tracingConfiguration
  type: object
- description: ''
  name: publish
  type: object
- description: ''
  name: versionDescription
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-update-state-machine-input-schema.json
slug: amazon-step-functions-update-state-machine-input
source_filename: amazon-step-functions-update-state-machine-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-state-machine-input-schema.json\",\n  \"title\": \"UpdateStateMachineInput\",\n  \"description\": \"UpdateStateMachineInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine.\"\n        }\n      ]\n    },\n    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Definition\"\n        },\n        {\n          \"description\": \"The Amazon States Language definition of the state machine. See <a href=\\\"https://docs.aws.amazon.com/step-functions/latest/dg/concepts-amazon-states-language.html\\\
  \">Amazon States Language</a>.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role of the state machine.\"\n        }\n      ]\n    },\n    \"loggingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingConfiguration\"\n        },\n        {\n          \"description\": \"Use the <code>LoggingConfiguration</code> data type to set CloudWatch Logs options.\"\n        }\n      ]\n    },\n    \"tracingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TracingConfiguration\"\n        },\n        {\n          \"description\": \"Selects whether X-Ray tracing is enabled.\"\n        }\n      ]\n    },\n    \"publish\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Publish\"\n        },\n        {\n  \
  \        \"description\": \"Specifies whether the state machine version is published. The default is <code>false</code>. To publish a version after updating the state machine, set <code>publish</code> to <code>true</code>.\"\n        }\n      ]\n    },\n    \"versionDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionDescription\"\n        },\n        {\n          \"description\": \"<p>An optional description of the state machine version to publish.</p> <p>You can only specify the <code>versionDescription</code> parameter if you've set <code>publish</code> to <code>true</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-state-machine-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: UpdateStateMachineInput
---
