---
description: ''
layout: schema
name: DescribeStateMachineOutput
properties_list:
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
  name: definition
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: creationDate
  type: object
- description: The <code>LoggingConfiguration</code> data type is used to set CloudWatch Logs options.
  name: loggingConfiguration
  type: object
- description: ''
  name: tracingConfiguration
  type: object
- description: ''
  name: label
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-describestatemachineoutput-schema.json
slug: step-functions-describestatemachineoutput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeStateMachineOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {},\n    \"name\": {},\n    \"status\": {},\n    \"definition\": {},\n    \"roleArn\": {},\n    \"type\": {},\n    \"creationDate\": {},\n    \"loggingConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"level\": {},\n        \"includeExecutionData\": {},\n        \"destinations\": {}\n      },\n      \"description\": \"The <code>LoggingConfiguration</code> data type is used to set CloudWatch Logs options.\"\n    },\n    \"tracingConfiguration\": {},\n    \"label\": {}\n  },\n  \"required\": [\n    \"stateMachineArn\",\n    \"name\",\n    \"definition\",\n    \"roleArn\",\n    \"type\",\n    \"creationDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-describestatemachineoutput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: DescribeStateMachineOutput
---
