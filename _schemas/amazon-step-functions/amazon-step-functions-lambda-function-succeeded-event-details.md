---
description: Contains details about a Lambda function that successfully terminated during an execution.
layout: schema
name: LambdaFunctionSucceededEventDetails
properties_list:
- description: ''
  name: output
  type: object
- description: ''
  name: outputDetails
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-lambda-function-succeeded-event-details-schema.json
slug: amazon-step-functions-lambda-function-succeeded-event-details
source_filename: amazon-step-functions-lambda-function-succeeded-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-lambda-function-succeeded-event-details-schema.json\",\n  \"title\": \"LambdaFunctionSucceededEventDetails\",\n  \"description\": \"Contains details about a Lambda function that successfully terminated during an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"The JSON data output by the Lambda function. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.\"\n        }\n      ]\n    },\n    \"outputDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoryEventExecutionDataDetails\"\n        },\n        {\n          \"description\"\
  : \"Contains details about the output of an execution history event.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-lambda-function-succeeded-event-details-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: LambdaFunctionSucceededEventDetails
---
