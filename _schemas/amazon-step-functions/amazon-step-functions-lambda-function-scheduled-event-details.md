---
description: Contains details about a Lambda function scheduled during an execution.
layout: schema
name: LambdaFunctionScheduledEventDetails
properties_list:
- description: ''
  name: resource
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: inputDetails
  type: object
- description: ''
  name: timeoutInSeconds
  type: object
- description: ''
  name: taskCredentials
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-lambda-function-scheduled-event-details-schema.json
slug: amazon-step-functions-lambda-function-scheduled-event-details
source_filename: amazon-step-functions-lambda-function-scheduled-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-lambda-function-scheduled-event-details-schema.json\",\n  \"title\": \"LambdaFunctionScheduledEventDetails\",\n  \"description\": \"Contains details about a Lambda function scheduled during an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the scheduled Lambda function.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"The JSON data input to the Lambda function. Length constraints apply to the payload size, and are expressed as bytes in\
  \ UTF-8 encoding.\"\n        }\n      ]\n    },\n    \"inputDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoryEventExecutionDataDetails\"\n        },\n        {\n          \"description\": \"Contains details about input for an execution history event.\"\n        }\n      ]\n    },\n    \"timeoutInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeoutInSeconds\"\n        },\n        {\n          \"description\": \"The maximum allowed duration of the Lambda function.\"\n        }\n      ]\n    },\n    \"taskCredentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskCredentials\"\n        },\n        {\n          \"description\": \"The credentials that Step Functions uses for the task.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-lambda-function-scheduled-event-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: LambdaFunctionScheduledEventDetails
---
