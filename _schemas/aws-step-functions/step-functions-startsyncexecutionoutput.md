---
description: ''
layout: schema
name: StartSyncExecutionOutput
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
  name: startDate
  type: object
- description: ''
  name: stopDate
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: error
  type: object
- description: ''
  name: cause
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
  name: billingDetails
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-startsyncexecutionoutput-schema.json
slug: step-functions-startsyncexecutionoutput
source_filename: step-functions-startsyncexecutionoutput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StartSyncExecutionOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {},\n    \"stateMachineArn\": {},\n    \"name\": {},\n    \"startDate\": {},\n    \"stopDate\": {},\n    \"status\": {},\n    \"error\": {},\n    \"cause\": {},\n    \"input\": {},\n    \"inputDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"included\": {}\n      },\n      \"description\": \"Provides details about execution input or output.\"\n    },\n    \"output\": {},\n    \"outputDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"included\": {}\n      },\n      \"description\": \"Provides details about execution input or output.\"\n    },\n    \"traceHeader\": {},\n    \"billingDetails\": {}\n  },\n  \"required\": [\n    \"executionArn\",\n    \"startDate\",\n    \"stopDate\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-startsyncexecutionoutput-schema.json
tags:
- iPaaS
- Orchestration
- Serverless
title: StartSyncExecutionOutput
---
