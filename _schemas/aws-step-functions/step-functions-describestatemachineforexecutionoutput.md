---
description: ''
layout: schema
name: DescribeStateMachineForExecutionOutput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: definition
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: updateDate
  type: object
- description: The <code>LoggingConfiguration</code> data type is used to set CloudWatch Logs options.
  name: loggingConfiguration
  type: object
- description: ''
  name: tracingConfiguration
  type: object
- description: ''
  name: mapRunArn
  type: object
- description: ''
  name: label
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-describestatemachineforexecutionoutput-schema.json
slug: step-functions-describestatemachineforexecutionoutput
source_filename: step-functions-describestatemachineforexecutionoutput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeStateMachineForExecutionOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {},\n    \"name\": {},\n    \"definition\": {},\n    \"roleArn\": {},\n    \"updateDate\": {},\n    \"loggingConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"level\": {},\n        \"includeExecutionData\": {},\n        \"destinations\": {}\n      },\n      \"description\": \"The <code>LoggingConfiguration</code> data type is used to set CloudWatch Logs options.\"\n    },\n    \"tracingConfiguration\": {},\n    \"mapRunArn\": {},\n    \"label\": {}\n  },\n  \"required\": [\n    \"stateMachineArn\",\n    \"name\",\n    \"definition\",\n    \"roleArn\",\n    \"updateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-describestatemachineforexecutionoutput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: DescribeStateMachineForExecutionOutput
---
