---
description: ''
layout: schema
name: GetExecutionHistoryInput
properties_list:
- description: ''
  name: executionArn
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: reverseOrder
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: includeExecutionData
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-getexecutionhistoryinput-schema.json
slug: step-functions-getexecutionhistoryinput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetExecutionHistoryInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {},\n    \"maxResults\": {},\n    \"reverseOrder\": {},\n    \"nextToken\": {},\n    \"includeExecutionData\": {}\n  },\n  \"required\": [\n    \"executionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-getexecutionhistoryinput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: GetExecutionHistoryInput
---
