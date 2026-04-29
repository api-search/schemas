---
description: ''
layout: schema
name: DescribeExecutionOutput
properties_list:
- description: ''
  name: executionArn
  type: object
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: startDate
  type: object
- description: ''
  name: stopDate
  type: object
- description: ''
  name: input
  type: object
- description: Provides details about execution input or output.
  name: inputDetails
  type: object
- description: ''
  name: output
  type: object
- description: Provides details about execution input or output.
  name: outputDetails
  type: object
- description: ''
  name: traceHeader
  type: object
- description: ''
  name: mapRunArn
  type: object
- description: ''
  name: error
  type: object
- description: ''
  name: cause
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-describeexecutionoutput-schema.json
slug: step-functions-describeexecutionoutput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeExecutionOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {},\n    \"stateMachineArn\": {},\n    \"name\": {},\n    \"status\": {},\n    \"startDate\": {},\n    \"stopDate\": {},\n    \"input\": {},\n    \"inputDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"included\": {}\n      },\n      \"description\": \"Provides details about execution input or output.\"\n    },\n    \"output\": {},\n    \"outputDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"included\": {}\n      },\n      \"description\": \"Provides details about execution input or output.\"\n    },\n    \"traceHeader\": {},\n    \"mapRunArn\": {},\n    \"error\": {},\n    \"cause\": {}\n  },\n  \"required\": [\n    \"executionArn\",\n    \"stateMachineArn\",\n    \"status\",\n    \"startDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-describeexecutionoutput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: DescribeExecutionOutput
---
