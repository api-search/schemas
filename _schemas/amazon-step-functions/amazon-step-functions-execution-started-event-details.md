---
description: Contains details about the start of the execution.
layout: schema
name: ExecutionStartedEventDetails
properties_list:
- description: ''
  name: input
  type: object
- description: ''
  name: inputDetails
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: stateMachineAliasArn
  type: object
- description: ''
  name: stateMachineVersionArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-execution-started-event-details-schema.json
slug: amazon-step-functions-execution-started-event-details
source_filename: amazon-step-functions-execution-started-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-execution-started-event-details-schema.json\",\n  \"title\": \"ExecutionStartedEventDetails\",\n  \"description\": \"Contains details about the start of the execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"The JSON data input to the execution. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.\"\n        }\n      ]\n    },\n    \"inputDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoryEventExecutionDataDetails\"\n        },\n        {\n          \"description\": \"Contains details about the input for an execution history\
  \ event.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role used for executing Lambda tasks.\"\n        }\n      ]\n    },\n    \"stateMachineAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies a state machine alias used for starting the state machine execution.\"\n        }\n      ]\n    },\n    \"stateMachineVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies a state machine version used for starting the state machine execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-execution-started-event-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: ExecutionStartedEventDetails
---
